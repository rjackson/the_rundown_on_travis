
# How do we allow certain failures?

```
language: ruby
rvm:
  - 2.0.0
  - jruby-19mode
script: rspec
matrix:
  allowed_failures:
    - rvm: jruby-19mode
```

https://travis-ci.org/rjackson/work_days/builds/15626132
