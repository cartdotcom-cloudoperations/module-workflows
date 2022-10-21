# Module Workflows
This repository provides re-usable workflows for Terraform modules.

## How To Use
Calling workflows in this repository is as simple as adding the following to a workflow file in the caller's repository:
```
jobs:
  call-workflow:
    uses: cartdotcom-cloudoperations/module-workflows/.github/workflows/<workflow-name>.yaml@main
    secrets: inherit
    with:
      <input>: <input-value>
```

## Resources
More information about workflow re-use can be found here: https://docs.github.com/en/actions/using-workflows/reusing-workflows
