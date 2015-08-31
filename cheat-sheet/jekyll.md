---
title: Jekyll Cheat Sheet
author: Danny Cheung
tags:
  - jekyll
  - cheat sheet
---

| Code | Description |
| ------- | ----------- |
| ```{{ "{{ variable_name " }} }}``` | Prints the value of <var>variable_name</var> |
| ```{{ "{% assign variable_name = value " }} %}``` | Assign the value <var>value</var> to <var>variable_name</var> |
| ```{{ "{{ variable_name | plus: value " }} }}``` | Print the value of <var>variable_name</var> increased by <var>value</var>. Does not update the value of <var>variable_name</var> |
| ```{{ "{% assign variable_name = variable_name | plus: value " }} %}``` | Increment the value of <var>variable_name</var> by <var>value</var>. |
| ```{{ "{% increment variable_name " }} %}``` | Increment variable <var>variable_name</var> by 1. If variable is new, value is 0. !! Separate variable scope to {{ "{% assign " }} %} tags !!|

## Resources

- http://jekyllrb.com/docs/configuration/
- https://docs.shopify.com/themes/liquid-documentation/basics
- https://mobilecommons.zendesk.com/hc/en-us/articles/202052544-Liquid-templates#comments
- http://cheat.markdunkley.com/
- http://stackoverflow.com/questions/3426182/how-to-escape-liquid-template-tags
