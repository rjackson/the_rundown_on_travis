
# Let me do that for you:

```sh
$ gem install travis
$ travis encrypt SOMEVAR=secretvalue
```

Then copy and paste into your `.travis.yml`.

To avoid copying & pasting:

```sh
$ travis encrypt api_token_value --add \
    notifcations.flowdock
```

