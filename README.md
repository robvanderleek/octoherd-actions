# octoherd-actions

Proof-of-concept repo for running [Octoherd scripts](https://github.com/octoherd/octoherd) with GitHub Actions.

## Generic Octoherd workflow for workflow dispatch events

The workflow file [`octoherd-workflow-dispatch.yml`](https://github.com/robvanderleek/octoherd-actions/blob/main/.github/workflows/octoherd-workflow-dispatch.yml) in this repo can be used to run arbitrary Octoherd scripts on workflow dispatch events.

The workflow can be started from the GitHub web UI or the [GitHub CLI](https://cli.github.com/):

```
[~/projects/octoherd-actions] $ gh workflow run
? Select a workflow Octoherd (octoherd.yml)
? script @octoherd/script-hello-world
? script_options --greeting-name World
✓ Created workflow_dispatch event for octoherd.yml at main
``` 

The output of the workflow run above can be viewed [here](https://github.com/robvanderleek/octoherd-actions/runs/5740114119?check_suite_focus=true).

## Generic Octoherd workflow for issue opened events

The workflow file [`octoherd-issue.yml`](https://github.com/robvanderleek/octoherd-actions/blob/main/.github/workflows/octoherd-issue.yml) in this repo can be used to run arbitrary Octoherd scripts on issue opened events.

The workflow can be started from [GitHub Issues](https://github.com/robvanderleek/octoherd-actions/issues/new/choose).
