
# RubyGems Deployment w/Custom Name

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: rubygems
  api_key: "YOUR API KEY"
  gem: my-gem-name
  on:
    tags: true
```
