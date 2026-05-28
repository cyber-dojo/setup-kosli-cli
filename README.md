
A composite workflow to setup the Kosli CLI.  

Typical use is as follows:

```yml
name: Main

...

jobs:
  setup:
    runs-on: ubuntu-latest
    steps:
      ...

      - uses: cyber-dojo/setup-kosli-cli@main
        with:
          version: "${{ vars.KOSLI_CLI_VERSION }}"

      ...
```
