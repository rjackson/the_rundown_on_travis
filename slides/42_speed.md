
# I feel the need, the need for speed!

## Tricks/Tips to speed up your builds...

* Cache packages. #1 speedup is not compiling C extensions.
  * Eliminates RubyGems SSL / Timeout issues.
  * Installing `nokogiri` alone takes 88 seconds!

* Remove non-essential gems from `Gemfile`/`gemspec`.

* Use matrix builds to speed up tests.
