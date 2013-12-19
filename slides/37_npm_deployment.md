
# NPM Deployment

```
language: js
ooe4
deploy:
  provider: npm
  email: "YOUR EMAIL ADDRESS"
  api_key: "YOUR API KEY"
  on:
    tags: true
```

```sh
travis encrypt ... --add deploy.api_key
```
