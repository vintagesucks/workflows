# workflows

This repository contains reusable GitHub Actions workflows.

## update-browserslist-data

This workflow updates Browserslist data, records the current target browsers in a `.browserslist.lock` file, and creates a pull request with any changes.

> [!NOTE]  
> This workflow only supports Yarn at the moment. Support for other package managers may be added in the future.

### Usage

```yaml
jobs:
  update-browserslist-data
    uses: vintagesucks/workflows/.github/workflows/update-browserslist-data.yml@update-browserslist-data/v2.0.0
    # with:
      # labels: 'yarn' # optional, defaults to 'dependencies,javascript'
    # secrets:
    #   token: ${{ secrets.PAT }} # optional, defaults to GITHUB_TOKEN
```

## update-yarn

This workflow updates Yarn to the latest version and creates a pull request with the changes.

### Usage

```yaml
jobs:
  update-yarn:
    uses: vintagesucks/workflows/.github/workflows/update-yarn.yml@update-yarn/v2.0.0
    # with:
      # labels: 'yarn' # optional, defaults to 'dependencies,javascript'
    # secrets:
    #   token: ${{ secrets.PAT }} # optional, defaults to GITHUB_TOKEN
```
