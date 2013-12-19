
# S3 Deployment Custom Folders

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
    local-dir: some-non-root-dir
    upload-dir: something-other-than-default
```

Will only upload the `/build` directory contents to S3.
