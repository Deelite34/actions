# actions

Collection of common Github actions used in our projects.


<!-- autogen -->


</br></br>

## deploy-backend

[action.yml](./deploy-backend/action.yml)

Deploys backend artifact to AWS.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |
| *no* | `artifact-path` | `string` | `"artifacts/backend/lambda.zip"` |  |
| **yes** | `aws-resource-name` | `string` | `""` |  |
| **yes** | `aws-cloudfront-id` | `string` | `""` |  |

</br></br>

## deploy-frontend

[action.yml](./deploy-frontend/action.yml)

Deploys frontend artifact to AWS.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |
| *no* | `artifact-path` | `string` | `"artifacts/frontend/"` |  |
| **yes** | `aws-resource-name` | `string` | `""` |  |
| **yes** | `aws-cloudfront-id` | `string` | `""` |  |

</br></br>

## pack-backend

[action.yml](./pack-backend/action.yml)

Packs backend for deployment and uploads artifact.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |
| **yes** | `environment-name` | `string` | `""` | environment name |
| *no* | `environment-url` | `string` | `""` | environment url |

</br></br>

## pack-frontend

[action.yml](./pack-frontend/action.yml)

Packs frontend for deployment and uploads artifact.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |
| **yes** | `environment-name` | `string` | `""` | environment name |
| *no* | `environment-url` | `string` | `""` | environment url |

</br></br>

## setup-backend

[action.yml](./setup-backend/action.yml)

Sets up runner environment for backend code.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |
| *no* | `python-version` | `string` | `"3.8"` | Python version to use |
| *no* | `pipenv-version` | `string` | `"2022.1.8"` | Pipenv version to use |

</br></br>

## setup-frontend

[action.yml](./setup-frontend/action.yml)

Sets up runner environment for frontend code.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |
| *no* | `cache-version` | `string` | `"1"` | Cache version used for invalidation |
| *no* | `node-version` | `string` | `"12"` | Node.js version to use |
| *no* | `yarn-version` | `string` | `"1.22.15"` | Yarn version to use |

</br></br>

## setup-infrastructure

[action.yml](./setup-infrastructure/action.yml)

Sets up runner environment for infrastructure code.

### inputs

| required? | name | type | default | description |
| --------- | ---- | ---- | ------- | ----------- |

