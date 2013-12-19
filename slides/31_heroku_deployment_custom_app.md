
# Heroku Deployment w/Custom App Name

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: heroku
  api_key: "YOUR API KEY"
  app: something-other-than-your-repo-name
```
