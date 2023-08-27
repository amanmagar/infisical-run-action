# Infisical run action

***Note: the scan workflow fails as the secret is delibrately kept on the workflow***

[![infisical scan test](https://github.com/amanmagar/infisical-test-repo/actions/workflows/infisical.yml/badge.svg?branch=main&event=push)](https://github.com/amanmagar/infisical-test-repo/actions/workflows/infisical.yml)


This action  helps to run infisical on the github actions.

Infisical is an open source secret-management tool to sync secrets across infrastructures. 

You can check out their project **[here](https://github.com/Infisical/infisical)**
## Inputs

## `command`

Supported commands:

```
infisical scan --verbose 

```     

**Required:** Specify the command to run on infisicals. Default `"--version"`. This command is used to show the infisical version to test if the infisical is installed or not by default.


## Example usage

```
uses: amanmagar/infisical-action@v1.0.0
with:
  command: scan --verboase

```

You can take the reference from  ***[this workflow](https://github.com/amanmagar/infisical-test-repo/actions/workflows/infisical.yml)***