## After forking upstream project, follow this instructions.

## git clone project into desire code folder
```git clone https://github.com/ggwiebe/e2e-mlops.git```

## Create new Python environment (using Conda)
```conda create --name=dbx-e2e-ml python=3.10```

## Switch to / Activate that environment
```conda activate dbx-e2e-ml```

## Install Databricks CLI
```pip install databricks-cli```

## Confirm db-cli connectivity
```databricks fs ls dbfs:/Users/glenn.wiebe@databricks.com/```
## check that files/directories are returned/printed

## Install Databricks dbx
```pip install dbx```

## Configure dbx project
```dbx configure --environment new-prod --profile e2-demo-west --workspace-dir /Shared/ggw_e2e_mlops/prod/dbx/e2e_mlops_prod --artifact-location dbfs:/Shared/ggw_e2e_mlops/prod/dbx/projects/e2e_mlops_dbx_prod```
