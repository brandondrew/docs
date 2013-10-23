---
layout: api-command 
language: Ruby
permalink: api/ruby/year/
command: year 
github_doc: https://github.com/rethinkdb/docs/edit/master/2-query-language/api/ruby/dates-and-times/year.md
related_commands:
    now: now/
    time: time/
---

{% apibody %}
time.year() → number
{% endapibody %}

Return the year of a time object.

__Example:__ Retrieve all the users born in 1986.

```rb
r.table("users").filter{ |user|
    user["birthdate"].year().eq(1986)
}.run(conn)

