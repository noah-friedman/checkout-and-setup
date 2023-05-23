# checkout-and-setup
Simple GitHub Action that checks out the repository and sets up the environment.

### USAGE
- Create a [composite action](https://docs.github.com/en/actions/creating-actions/creating-a-composite-action) in the same repository as the workflow using this action.
  The file should be at the path `.github/actions/setup/action.yml` relative to the repository root.
- Make sure the local `setup` action takes an input `secrets` if you require any secrets in this action. Use retrieve values from `inputs.secrets` instead of `secrets`.
- Run this action in your workflow, providing `secrets` input if necessary.
