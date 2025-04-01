# workflows

This repository contains reusable GitHub Actions workflows.

## update-yarn

This workflow updates Yarn to the latest version and creates a pull request with the changes.

### Usage

```yaml
jobs:
  update-yarn:
    uses: vintagesucks/workflows/update-yarn@update-yarn/v1.0.1
    secrets:
      token: ${{ github.token }}
```
