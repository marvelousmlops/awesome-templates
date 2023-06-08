# set_env_vars

### What it does:
- gets some inputs
- creates env variables for given inputs and git sha
- created environment variables accessible in next steps in github workflow job:
  - USER_NAME
  - DATABRICKS_HOST
  - GIT_TAG
  - PROJECT_NAME

### Required inputs:

#### user name
User name

#### databricks host
Databricks workspace url

### Usage
```
  - name: Set up env vars
    id: set_env_vars
    uses: marvelousmlops/awesome-templates/.github/actions/set_env_vars@master
    with:
      user_name: ${{ secrets.USER_NAME }}
      databricks_host: ${{ secrets.DATABRICKS_HOST }}
```
