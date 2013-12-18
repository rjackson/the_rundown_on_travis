
# Whatever, I've got custom setup steps.

* Simply specify your install steps:

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
```

https://travis-ci.org/rjackson/work_days/builds/15624742

???

Run the same as last time, but also run the following before 
rspec:

* `sudo apt-get update && sudo apt-get install git`
* `gem install bundler --pre`
