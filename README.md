# dummy-api

Simple util for having a dummy RESTful API. No database necessary, this is just to aid in development of clientside apps.

I just never wanted to do this again and it's useful for me in more than one project.


## installing

npm i dummy-api


## using

```js
var express = require('express');
var app = express();

var api = require('dummy-api');

app.get('/api/people', api.list);
app.get('/api/people/:id', api.get);
app.delete('/api/people/:id', api.delete);
app.put('/api/people/:id', api.update);
app.post('/api/people', api.add);

app.listen(3000);
```

## license

MIT

## credits

Written by [@HenrikJoreteg](http://twitter.com/henrikjoreteg).
