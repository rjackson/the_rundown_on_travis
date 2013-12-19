
# Heroku Deployment w/After Deploy

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: heroku
  api_key: "YOUR API KEY"
  run:
    - "rake db:migrate"
    - "rake cleanup"
```
