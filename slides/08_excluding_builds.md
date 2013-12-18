
# How do we skip a build?

```
language: ruby
rvm:
  - 2.0.0
  - jruby-19mode
script: rspec
env:
  - AWESOME_VAR=hell-yeahz
  - WHAT_EVES=shut-up
matrix:
  exclude:
    - rvm: jruby-19mode
      env: AWESOME_VAR=hell-yeahz
    - rvm: 2.0.0
      env: WHAT_EVES=shut-up
```

https://travis-ci.org/rjackson/work_days/builds/15625669
