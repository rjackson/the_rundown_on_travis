
# RubyGems Deployment -- Prereleases

```
language: ruby
rvm:
  - 2.0.0
script: rspec
deploy:
  provider: rubygems
  api_key: "YOUR API KEY"
```

```ruby
# in your gemspec (with less wrapping)
if ENV['TRAVIS']
  s.version = "#{s.version}-alpha-" + 
            ENV['TRAVIS_BUILD_NUMBER']
end
```
