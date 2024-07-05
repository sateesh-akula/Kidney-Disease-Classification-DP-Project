# Kidney-Disease-Classification-DP-Project

## Workflows
 1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the dvc.yaml
10. app.py

# How to run?

### STEPS

Clone the repo

```bash
https://github.com/sateesh-akula/Kidney-Disease-Classification-DP-Project
```

### STEP 1 - Create an conda environment after opening the repo

```bash
conda create -n dummyname python=3.8 -y
```

```bash
conda activate dummyname
```

### STEP 2 - Install the requirments
```bash
pip install -r requirements.txt
```



## MLflow

- [Documentation](https://mlflow.org/docs/latest/index.html)


##### cmd
- mlflow ui


### DagsHub
[Official-Page](https://dagshub.com/)

1. Connect your repo from github to dagshub
2. In Dagshub Repo, remote -> Experiments
3. Copy Mlflow URI ["https://dagshub.com/username/repo"]
4. Copy the following from mlflow tracking, Which goes similar to this.

    ```bash
    import dagshub
    dagshub.init(repo_owner=" ",repo_name=" ",mlflow=True)
    ```
5. Add it to the main.py 

[`Note`: Dagshub will ask for authentication, it is recommened to clone repo and try it.]

### DVC commands [For Data Pipeline]

- [DVC Documentation Page](https://dvc.org/doc/command-reference)

1. dvc init
2. dvc repro
3. dvc dag



