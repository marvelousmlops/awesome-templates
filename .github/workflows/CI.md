# CI

### What it does:
- Installs dependencies from requirements.txt file
- Runs pytest

### Required inputs:

#### requirements file
Requirements file name for dependencies

#### test dir
Directory for tests

### Usage
```
  - name: Your-Project-Name
    on: [push]
    jobs:
    YOUR-JOB-NAME-HERE:
        uses: marvelousmlops/awesome-templates/.github/workflows/CI.yml@COMMIT_HASH_YOU_WANT_TO_USE
        with:
            requirements_file: "requirementx.txt"
            test_dir: "tests/"
```