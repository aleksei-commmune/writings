# CI

## Old workflow

- Linting everything
- Unit-tests only for everything, no matter what was changed
- No tests

## New workflow

- The brand-new concept
- Split by monorepo folders: lint and tests
- path filtering for save
- e2e as a separate workflow
- use composite actions as functions in the code

## E2E

- On push vs before merge
- matrix approach to run tests in parallel

## Money saving technics

- ChatGPT knows. But use it wisely, almost all the time you can ask it something like "please make it simple" or "simplify" and a suggested solution becomes much more. And reformulate your request if the answers seem strange or inappropriate. Don't forget to think :smile:
- because of the big dependency base and monorepo structure
- combine linting and testing jobs into the single job
- move small steps to the job itself even if it will do the task several times
- move everything you can outside of the matrix
- extensions for vs code
  - [GitHub Actions](https://marketplace.visualstudio.com/items?itemName=cschleiden.vscode-github-actions)

## Problems

- Deprecations
- Required workflows (path filtering)
- Testing wastes money - consider using some repo with a similar project structure as a playground

## Next steps

- CD
- Using some build system to simplify the CI
- Optimization of build and run services and containers
