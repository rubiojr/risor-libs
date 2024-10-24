# RSX

RSX https://github.com/rubiojr/rsx) utility library.

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
