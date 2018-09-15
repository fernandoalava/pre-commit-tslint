# pre-commit-tslint
Just another tslint hook for [pre-commit](https://github.com/pre-commit/pre-commit)

# How to use
- Install [pre-commit](https://pre-commit.com/#install)
- In the root directory of your project add a new file with this name `.pre-commit-config.yaml`
- Add the following lines in the file:

```
- repo: https://github.com/fernandoalava/pre-commit-tslint
  rev: 1.0.3 # always use the last version
  hooks:
    - id: tslint
      args: ['--project','tsconfig.json'] # you can add more parameters if you require, the tsconfig.json must have all rules for your project.
```
