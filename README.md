# Risor Libraries

[Risor](https://risor.io) unofficial libraries.

## GitHub

GitHub client library.

```risor
import github as gh
import os

gh.set_token(os.getenv("GITHUB_TOKEN"))
me := gh.me()
print(me.login)
```

## Test

Risor library to write tests.

```risor
import test

test.is_true("this test will not fail", true)

test.raises("this test should raise a boom error", func(){
  error("boom")
}, errors.new("boom"))

test.nothing_raised("this test should raise a boom error", func(){
  true
})
```

## RMM (Risor Module Manager)

Risor library to manage third-party libraries.

```risor
import rmm

// Download rsx.risor if not already downloaded and import it.
// The default installation path is $HOME/.local/share/risor/modules, but you can change it with the install_path option.
rmm.load(
  "gh:rubiojr/risor-libs/lib/rsx",
  { force: true, branch: "main" } // force means re-download (overwrite/update)
)

import rsx
```

## RSX

[RSX](https://github.com/rubiojr/rsx) utility library.
