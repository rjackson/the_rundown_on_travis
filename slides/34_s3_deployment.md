
# S3 Deployment

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
```

```sh
$ travis encrypt ... --add deploy.secret_access_key
$ travis encrypt ... --add deploy.access_key_id
```

???

OR

```
 $ travis setup s3
```
