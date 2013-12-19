
# Custom Deployment Script

```
language: js
node_js:
  - 0.10
script: grunt test
after_success:
  - grunt deploy
```

https://travis-ci.org/rjackson/ember-live-api/builds/15688141
