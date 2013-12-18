
# Conditional email notifications:

```
language: ruby
rvm:
  - 2.0.0
script: rspec
notifications:
  email:
    on_success: always
    on_failure: always
```

https://travis-ci.org/rjackson/work_days/builds/15670128

???

on_success defaults to change
on_failure defaults to always
