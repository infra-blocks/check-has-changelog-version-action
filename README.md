<<<<<<< HEAD
# check-has-changelog-version-action
[![Release](https://github.com/infra-blocks/check-has-changelog-version-action/actions/workflows/git-tag-semver-from-label.yml/badge.svg)](https://github.com/infra-blocks/check-has-changelog-version-action/actions/workflows/git-tag-semver-from-label.yml)
[![Self Test](https://github.com/infra-blocks/check-has-changelog-version-action/actions/workflows/self-test.yml/badge.svg)](https://github.com/infra-blocks/check-has-changelog-version-action/actions/workflows/self-test.yml)
[![Update From Template](https://github.com/infra-blocks/check-has-changelog-version-action/actions/workflows/update-from-template.yml/badge.svg)](https://github.com/infra-blocks/check-has-changelog-version-action/actions/workflows/update-from-template.yml)
=======
# composite-action-template
[![Release](https://github.com/infra-blocks/composite-action-template/actions/workflows/git-tag-semver-from-label.yml/badge.svg)](https://github.com/infra-blocks/composite-action-template/actions/workflows/git-tag-semver-from-label.yml)
[![Self Test](https://github.com/infra-blocks/composite-action-template/actions/workflows/self-test.yml/badge.svg)](https://github.com/infra-blocks/composite-action-template/actions/workflows/self-test.yml)
[![Update Template Instances](https://github.com/infra-blocks/composite-action-template/actions/workflows/trigger-update-from-template.yml/badge.svg)](https://github.com/infra-blocks/composite-action-template/actions/workflows/trigger-update-from-template.yml)
>>>>>>> template/master

This action enforces that the changelog has a section for the version that is provided as an input. If it
doesn't, the action fails.

This can be useful, for example, when making sure developers add a changelog entry for a new
version before releasing said version.

## Inputs

|      Name      | Required | Description                                                                                                                |
|:--------------:|:--------:|----------------------------------------------------------------------------------------------------------------------------|
| changelog-file |  false   | Where to find the changelog. See [parse-changelog-action](https://github.com/infra-blocks/parse-changelog-action) |
|    version     |   true   | The version to find in the changelog. The action will fail when this version is absent.                                    |

## Outputs

|      Name      | Description                                                                                                                      |
|:--------------:|----------------------------------------------------------------------------------------------------------------------------------|
| changelog-file | The effective changelog-file used. See [parse-changelog-action](https://github.com/infra-blocks/parse-changelog-action) |


## Permissions

N/A

## Usage

```yaml
jobs:
  stuff:
    runs-on: ubuntu-22.04
    steps:
<<<<<<< HEAD
      - uses: infra-blocks/check-has-changelog-version-action@v1
        with:
          changelog-file: MY-CHANGELOG.md
          version: 1.0.0
=======
      - uses: infra-blocks/composite-action-template@v1
>>>>>>> template/master
```
