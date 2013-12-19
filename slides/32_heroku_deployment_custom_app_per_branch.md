
# Heroku Deployment per Branch

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: heroku
  api_key: "YOUR API KEY"
  app:
    master: dont-touch-the-red-button
    staging: not-so-sure-about-this
    production: ship-it-city
```

