
# Caching with WAD

* Get the script:

```bash
$ curl -o bin/wad \
  https://raw.github.com/Fingertips/WAD/master/bin/wad
$ chmod +x bin/wad
```

Then use `bin/wad` instead of `bundle install`:

```
language: ruby
install: bin/wad
script: rspec
```
