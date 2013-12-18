
# Custom IRC Notifications

```
language: ruby
rvm:
  - 2.0.0
script: rspec
notifications:
irc:
  channels:
    - "chat.freenode.net#rwjblue"
  template:
    - "%{repository}#%{build_number} (%{branch} - %{commit} : %{author}): %{message}"
    - "Change view : %{compare_url}"
    - "Build details : %{build_url}"
```

???

You can interpolate the following variables:

repository: your GitHub repo URL
build_number: build number
branch: branch build name
commit: shortened commit SHA
author: commit author name
message: travis message to the build
compare_url: commit change view URL
build_url: URL of the build detail
