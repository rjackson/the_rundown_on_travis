
# Webhook Authorization Header

```ruby
require 'digest'

sha = Digest::SHA2.new
sha << 'rjackson/work_days' + TRAVIS_TOKEN
sha.hexdigest
```

```python
from hashlib import sha256

sha256('rjackson/work_days' + TRAVIS_TOKEN).hexdigest()
```
