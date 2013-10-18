---
layout: api-command 
language: JavaScript
permalink: api/javascript/mul/
command: mul
github_doc: https://github.com/rethinkdb/docs/edit/master/2-query-language/api/javascript/math-and-logic/mul.md
---

{% apibody %}
number.mul(number) → number
array.mul(number) → array
{% endapibody %}

Multiply two numbers, or make a periodic array.

__Example:__ It's as easy as 2 * 2 = 4.

```js
r.expr(2).mul(2).run(conn, callback)
```

__Example:__ Arrays can be multiplied by numbers as well.

```js
r.expr(["This", "is", "the", "song", "that", "never", "ends."]).mul(100).run(conn, callback)
```
