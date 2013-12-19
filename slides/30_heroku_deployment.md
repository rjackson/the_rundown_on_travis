
# Heroku Deployment

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: heroku
  api_key: "YOUR API KEY"
```

Populate the secure API key:

```
travis encrypt $(heroku auth:token) --add deploy.api_key
```
