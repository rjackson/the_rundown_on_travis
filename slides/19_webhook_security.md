
# Webhook Authorization Header

```ruby
require 'digest'
Digest::SHA2.hexdigest('rjackson/work_days' + 
                        TRAVIS_TOKEN)
```

```python
from hashlib import sha256

sha256('rjackson/work_days' + TRAVIS_TOKEN).hexdigest()
```
