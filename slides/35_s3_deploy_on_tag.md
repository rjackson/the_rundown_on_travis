
# S3 Deployment on Tags

```
language: ruby
rvm:
  - 2.0.0
  script: rspec
  deploy:
    provider: s3
    access_key_id: "YOUR AWS ACCESS KEY"
    secret_access_key: "YOUR AWS SECRET KEY"
    bucket: "S3 Bucket"
    skip_cleanup: true
  'on':
    tags: true
```

'on' - WTF?

https://gist.github.com/rjackson/6700004
