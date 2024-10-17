# Risor Libraries

[Risor](https://risor.io) unofficial Risor native libraries.

## Worker pool

Simple worker pool to run arbitrary functions.

```Go
import pool
// Create a pool with 2 workers
pool.new(2)

// Queue up some jobs
for range 10 {
  pool.queue(func() { time.sleep(1); print("hello") })
}

// Wait for all jobs to finish
pool.wait()
```

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

```Go
import test

test.is_true("this test will not fail", true)

test.raises("this test should raise a boom error", func(){
  error("boom")
}, errors.new("boom"))

test.nothing_raised("this test should raise a boom error", func(){
  true
})
```

## RSX

[RSX](https://github.com/rubiojr/rsx) utility library.

```Go
import

// Download rsx.risor if not already downloaded and import it.
// The default installation path is $HOME/.local/share/risor/modules, but you can change it with the install_path option.
rmm.load(
  "gh:rubiojr/risor-libs/lib/test",
  { force: true, branch: "main" } // force means re-download (overwrite/update)
)

import test

test.is_true("/tmp is a directory", rsx.is_dir("/tmp"))

```
