---
layout: panel
title: Practice contests
id: practice_contests
---

## Past practice contests

We currently organize weekly practice contest to improve our skills for [NCPC](https://nordic.icpc.io) and beyond. Normally we meet up at Thursdays at 17:15 in the room E:2116. To find out if there will be a training session this week check out the `#progträningar` channel in our discord. 

This is a list of links to practice contests:

{% assign sorted_contest = site.data.practice_contests | sort: "date" | reverse %}

<table id="my-table">
{% for contest in sorted_contest %}
<tr>
<td>
{{ contest.date }}
</td>
<td>
{{ contest.name }}
</td>
<td>
<a href="{{ contest.link }}">{{contest.link}}</a>
</td>
</tr>
{% endfor %}
</table>

<style>
#my-table td {
    padding: 2px 2px;
}
#my-table tr:hover {

}
</style>