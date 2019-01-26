### davis.js
---
https://github.com/olivernn/davis.js

```js
var app = Davis(function(){
  this.get('/welcome/:name', function(req){
    $('body').append('' + req.params['name'] + '!</h1>')
  })
})
$(document).ready(function(){
  $('body').append('<a href="welcome/bob">Greet</a>');
  app.start();
})
```

```
make test
curl http://localhost:3000/examples/todo.html
```

```
```

