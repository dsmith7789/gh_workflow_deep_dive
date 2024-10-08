# Events: Detailed control over when workflows are triggered:

## Available Events:
* Most are repository related (ex. `pull_request`, `push`)
* Some are more general (ex. `schedule`)

## Activity Types:
Ex: `pull_request` event => `opened, closed, edited, etc.`

## Filters:
Ex: `push` event => Filter based on target branch.
* `paths-ignore`: If any file in this path changed, don't trigger workflow
* `paths`: If any file in one of the listed paths changed, trigger the workflow

## Forks and Pull Requests:
First time contributors must be approved manually. This avoids security risks. Anyone can fork and create pull requests for public repos, so a malicious actor could trigger excessive workflows on your repo.

## Cancelling Workflows
* Cancelled by default if jobs or steps fail
* Can also be cancelled manually

## Skipping Workflows
* Don't trigger a workflow in cases where it would normally get triggered
* Use proper commit message "`[skip ci]`" "`[skip actions]`"