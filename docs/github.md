# GitHub

GitHub client library.

```Go
import github as gh
import os

gh.set_token(os.getenv("GITHUB_TOKEN"))
me := gh.me()
print(me.login)
```

