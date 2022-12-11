# Setup OVR Platform Util

A GitHub Action to setup the ovr platform utility tool

## How to use

```yaml
jobs:
  validate:
    runs-on: ${{ matrix.os }}
    strategy:
      matrix:
        os: [ macos-latest, windows-latest, macos, windows ]

    steps:
        # download and setup ovr platform util
      - uses: RageAgainstThePixel/setup-ovr-platform-util@v1

        # run commands
      - run: 'ovr-platform-util version'
        shell: pwsh
```
