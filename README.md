
A composite workflow to setup the Kosli CLI.  
A wrapper for `kosli-dev/setup-cli-action` allowing its version to be
bumped here, in one place. The input.version defaults to `latest`

Typical use is with other standard job setup steps:

```yml
name: Main

...

jobs:
  setup:
    runs-on: ubuntu-latest
    steps:
      ...
      - uses: cyber-dojo/harden-runner@main
      - uses: cyber-dojo/setup-kosli-cli@main
      - uses: cyber-dojo/pinned-checkout@main

      ...
```
