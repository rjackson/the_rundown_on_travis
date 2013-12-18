
# Webhooks

```
language: ruby
rvm:
  - 2.0.0
script: rspec
notifications:
  webhooks: http://your-domain.com/notifications
```

???

The URL provided will be posted to with a JSON payload including 
all of the build details (including pass/fail).

https://gist.github.com/svenfuchs/1225015
