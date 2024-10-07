# Events: Detailed control over when workflows are triggered:
## Activity Types:
Ex: `pull_request` event => `opened, closed, edited, etc.`

## Filters:
Ex: `push` event => Filter based on target branch.
* `paths-ignore`: If any file in this path changed, don't trigger workflow
* `paths`: If any file in one of the listed paths changed, trigger the workflow