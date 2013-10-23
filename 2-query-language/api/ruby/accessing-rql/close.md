---
layout: api-command 
language: Ruby
permalink: api/ruby/close/
command: close 
github_doc: https://github.com/rethinkdb/docs/edit/master/2-query-language/api/ruby/accessing-rql/close.md
related_commands:
    connect: connect/
    use: use/
    repl: repl/
    reconnect: reconnect/
---

{% apibody %}
connection.close
{% endapibody %}

Close an open connection. Closing a connection cancels all outstanding requests and frees
the memory associated with the open requests.

__Example:__ Close an open connection.

```rb
conn.close
```

