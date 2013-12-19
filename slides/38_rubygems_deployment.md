
# RubyGems Deployment

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: rubygems
  api_key: "YOUR API KEY"
  on:
    tags: true
```

```sh
travis encrypt --add deploy.api_key
```
