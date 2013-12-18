
# Specifying custom environment variables:

```
language: ruby
rvm:
  - 2.1.0
  - 2.0.0
  - 1.9.3
  - jruby-19mode
before_install:
  - sudo apt-get update && sudo apt-get install git
  - gem install bundler --pre
script: rspec
env:
  global:
    - AWESOME_VAR=hell-yeahz
    - WHAT_EVES=shut-up
```

https://travis-ci.org/rjackson/work_days/builds/15665245

???

Note that these are global variables. They do not create mutiple builds.
