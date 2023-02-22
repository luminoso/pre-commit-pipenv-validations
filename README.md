[pre-commit](https://pre-commit.com/) hooks to for basic [pipenv](https://pipenv-fork.readthedocs.io/) validations

## Usage

```yaml
---
repos:
  - repo: https://github.com/luminoso/pre-commit-pipenv-validations
    rev: v1.0.0
    hooks:
      - id: pipenv_check
      - id: pipenv_verify
```

## Tests supported

|     **id**      |  **Requires**  |                               **Description**                               |
| :-------------: | :------------: | :-------------------------------------------------------------------------: |
| `pipenv_check`  | `Pipfile.lock` | Checks for PyUp Safety security vulnerabilities and against PEP 508 markers |
| `pipenv_verify` |   `Pipfile`    |                Verify the hash in Pipfile.lock is up-to-date                |

# Licence

MIT
