
# Build Lifecycle Hooks

* before_install
* install
* before_script
* script
* after_success/after_failure
* after_script

???

Any non `after` script exiting non-zero indicates
a failure.

As we saw earlier any of these can be an array.
