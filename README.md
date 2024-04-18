# check-changelog-has-version-action
[![Release](https://github.com/infrastructure-blocks/check-changelog-has-version-action/actions/workflows/git-tag-semver-from-label.yml/badge.svg)](https://github.com/infrastructure-blocks/check-changelog-has-version-action/actions/workflows/git-tag-semver-from-label.yml)
[![Self Test](https://github.com/infrastructure-blocks/check-changelog-has-version-action/actions/workflows/self-test.yml/badge.svg)](https://github.com/infrastructure-blocks/check-changelog-has-version-action/actions/workflows/self-test.yml)
[![Update From Template](https://github.com/infrastructure-blocks/check-changelog-has-version-action/actions/workflows/update-from-template.yml/badge.svg)](https://github.com/infrastructure-blocks/check-changelog-has-version-action/actions/workflows/update-from-template.yml)

Upon creating a repository from this template:
- Edit the action.yml to correspond to your new action
- Edit the self-test workflow.
- Document

## Inputs

|     Name      | Required | Description       |
|:-------------:|:--------:|-------------------|
| example-input |   true   | An example input. |

## Outputs

|      Name      | Description        |
|:--------------:|--------------------|
| example-output | An example output. |

## Permissions

|     Scope     | Level | Reason   |
|:-------------:|:-----:|----------|
| pull-requests | read  | Because. |

## Usage

```yaml
name: Template Usage

on:
  push: ~

# The required permissions.
permissions:
  pull-requests: read

# The suggested concurrency controls.
concurrency:
  group: ${{ github.workflow }}-${{ github.ref }}
  cancel-in-progress: true

jobs:
  example-job:
    runs-on: ubuntu-22.04
    steps:
      - uses: infrastructure-blocks/check-changelog-has-version-action@v1
```
