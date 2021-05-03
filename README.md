# github-actions-artifacts-test

Test repository to showacase the creation of assets using a [GitHub Action Workflow matrix](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idstrategymatrix) and then combination and automated release using [@semantic-release](https://github.com/semantic-release/)

There are two GitHub Action workflows in this repository:

1. [`.github/workflows/build.yml`](.github/workflows/build.yml): Building the assets on demand, using [the `workflow_dispatch` trigger](https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/).
2. [`.github/workflows/release.yml`](.github/workflows/release.yml): same as the build workflow, but also creates an automated release and uploads all files created in the build matrix to the GitHub release.

## License

[ISC](LICENSE)
