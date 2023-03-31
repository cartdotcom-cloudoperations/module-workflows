# Module Workflows
This repository provides re-usable workflows for Terraform modules.

Calling workflows in this repository is as simple as adding the following to a workflow file in the caller's repository:
```
jobs:
  call-workflow:
    uses: cartdotcom-cloudoperations/module-workflows/.github/workflows/<workflow-name>.yaml@main
    secrets: inherit
    with:
      <input>: <input-value>
```

More information about workflow re-use can be found here: https://docs.github.com/en/actions/using-workflows/reusing-workflows

## Workflows
### CI Workflow

The reusable CI workflow (`.github/workflows/CI.yaml`) abstracts the process of validating the correctness of Terraform modules before they are deployed. It also automates the release process should the CI process succeed. For more information about what's happening, view the workflow code directly.