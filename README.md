# Snakemake workflow: `<name>`

This repository is only meant for testing out the required minimal permissions to get GitHub Actions CI workflows to run on release-please pull requests.

## Steps to get `release-please` to successfully open a pull request

1. Allow GitHub Actions to open and approve pull requests via `Settings -> Actions -> General -> Workflow permissions -> [] Allow GitHub Actions to create and approve pull requests`:
   https://github.com/googleapis/release-please-action?tab=readme-ov-file#workflow-permissions
2. Specifically give the release-please Action permission to read and write `contents:` and `pull-requests:`:
   ```
   permissions:
     contents: write
     pull-requests: write
   ```
