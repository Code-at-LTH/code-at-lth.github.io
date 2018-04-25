---
layout: panel
title: Grid BFS
---

## BFS in Grids

### Problems
- [Grid](https://open.kattis.com/problems/grid)
- [Coast Length](https://open.kattis.com/problems/coast)
- [Terraces](https://open.kattis.com/problems/terraces)
- [Dacey the Dice](https://open.kattis.com/problems/daceydice)
- [Wet Tiles](https://open.kattis.com/problems/wettiles)
- [Fire](https://open.kattis.com/problems/fire2)
- [10 Kinds of People](https://open.kattis.com/problems/10kindsofpeople)
- [Horror List](https://open.kattis.com/problems/horror)
- [Lava](https://open.kattis.com/problems/lava)
- [Zoning](https://open.kattis.com/problems/zoning)
- [Pokémon Ice Maze](https://open.kattis.com/problems/pokemon)

Breath First Search is a technique to find shortest paths in unweighted graphs. All nodes are preccessed in order of how far away they are from the starting node. Todo this, commonly we use a FIFO-queue. In python deque is a double ended queue and can be used as a FIFO-queue. This week we will focus on grids, and view them as graphs. All the neighbours of a grid cell is easy to find, there are at most 4, all the adjacent cells. The following code performs a BFS from the cell `(startx, starty)`, in an `N` by `M` grid.

```python
from collections import deque
def BFS(startx, starty):
    q = deque([(startx, starty)])
    dist = {(startx, starty): 0}
    while q:
        x, y = q.popleft()
        for nx, ny in [(x + 1, y), (x - 1, y), (x, y + 1), (x, y - 1)]:
            if 0 <= nx < N and 0 <= ny < M:
                coord = nx, ny
                if coord not in dist:
                    dist[coord] = dist[x, y] + 1
                    q.append(coord)
    return dist
```

However, this is not of any use yet, since the manhattan distance can be calculated directly. This code is however of use if the grid has cells that are forbidden to visit. Then those cells can be filtered out at the same place as cells outside the grid are filtered out now. Then we can find the shortest distance in a maze.
