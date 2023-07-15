## WHAT
this is a generic, reusable GitHub workflow that aims to address ~80% of modern application deployment use cases

## WHY
standardized workflows (i.e., CI/CD pipelines) help ensure consistancy and ease of use

## WHO
everyone!

## MORE
many decisions were made to enforce devops best practies. these decisions, and their justification, have been listed below.

decision: an environment is required in order to accomplish anything
reason: as many "quality gates" can be enabled with environments in GitHub, environments are required in order to prevent malicious or accidental deployments without explicit approval.

use it like this 

``` yaml
jobs:
  <your-job-here>:
    uses: chenette/workflow/main.yml@main
    with:
      environment: <your-environment-here>
      ...
```