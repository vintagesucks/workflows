# workflows

This repository contains reusable GitHub Actions workflows.

## update-yarn

This workflow updates Yarn to the latest version and creates a pull request with the changes.

### Usage

```yaml
jobs:
  update-yarn:
    uses: vintagesucks/workflows/.github/workflows/update-yarn.yml@update-yarn/v1.0.0
    # secrets:
    #   token: ${{ secrets.PAT }} # optional, defaults to GITHUB_TOKEN
```
