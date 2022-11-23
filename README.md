# My Debian package

Yet another "build my package" Github's actions.

## Usage

Example

```yaml
---

name: Build Debian package

on:
  push:
    branches: [ "main" ]

jobs:

  package:
    runs-on: ubuntu-latest

    steps:
      - name: my Debian package
        # You may pin to the exact commit or the version.
        # uses: deogracia/my-debian-package@33b6b656bd669388d02dbf39c052f70f76943e8f
        uses: deogracia/my-debian-package@v0.2.0
        with:
          # Input to use
          myInput: # optional, default is world
```
