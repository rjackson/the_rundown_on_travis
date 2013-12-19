
# Securing Secrets

* Each repo is given a key pair:

  https://api.travis-ci.org/repos/rjackson/work_days/key

* Use the public key to encrypt the secret data in your `.travis.yml`.

* Use `secret: <ENCRYPTED_STRING>`
