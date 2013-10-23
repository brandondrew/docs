---
layout: api-command 
language: JavaScript
permalink: api/javascript/month/
command: month
github_doc: https://github.com/rethinkdb/docs/edit/master/2-query-language/api/javascript/dates-and-times/month.md
io:
    -   - time
        - number
related_commands:
    now: now/
    time: time/
---


{% apibody %}
time.month() → number
{% endapibody %}

Return the month of a time object as a number between 1 and 12. For your convenience, the terms r.january, r.february etc. are defined and map to the appropriate integer.

__Example:__ Retrieve all the users who were born in November.

```js
r.table("users").filter(
    r.row("birthdate").month().eq(11)
)
```


__Example:__ Retrieve all the users who were born in November.

```js
r.table("users").filter(
    r.row("birthdate").month().eq(r.november)
)
```
