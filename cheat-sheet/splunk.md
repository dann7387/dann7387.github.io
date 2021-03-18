---
title: Splunk Cheat Sheet
author: Danny Cheung
tags:
  - splunk
  - cheat sheet
---

| Command | Description |
| ------- | ----------- |
| ```earliest=<MM/DD/YYYY:hh:mm:ss> latest=<MM/DD/YYYY:hh:mm:ss>``` | Restrict result to a time range via search query |
| ```<bas_search> \| stats count by <agg_field> \| eventstats sum(count) as total \| eval percent=round(100*count/total,2) \| sort -percent``` | Sort entries as a percentage of all entries |
