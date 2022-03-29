# octoherd-actions

Proof-of-concept repo for running [Octoherd scripts](https://github.com/octoherd/octoherd) with GitHub Actions.

## Generic Octoherd workflow

The workflow file [`octoherd.yml`](https://github.com/robvanderleek/octoherd-actions/blob/main/.github/workflows/octoherd.yml) in this repo can be used to run
arbitrary Octoherd scripts.

The workflow can be started from the GitHub web UI or the [GitHub CLI](https://cli.github.com/):

```
[~/projects/octoherd-actions] $ gh workflow run
? Select a workflow Octoherd (octoherd.yml)
? script @octoherd/script-hello-world
? script_options --greeting-name World
✓ Created workflow_dispatch event for octoherd.yml at main
``` 

The output of the workflow run above can be viewed [here](https://github.com/robvanderleek/octoherd-actions/runs/5740114119?check_suite_focus=true).
