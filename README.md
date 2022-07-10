# CI/CD Monorepo

To use CI/CD pipelines in this repo, reference the pipeline in the repository settings:

`Settings  -> CI/CD -> General Pipelines -> CI/CD configuration file`

and replace the placeholder with `path/to/pipeline.yaml@git_repo_path`

For exmpale:

`python/pipeline.yaml@/cloudlet/repo-templates/ci-cd-pipeline`

Then, add the variables for the CI/CD:

`Settings -> CI/CD -> General Pipelines -> Variables`

| Variable     | Example      | Description  |
| :------------ |   :---:       | --------: |
| `APP`        | tester         |Applictaion name   |
| `HELM_GIT_PATH`| cloudlet/helm/tester         | Helm chart git path   |
