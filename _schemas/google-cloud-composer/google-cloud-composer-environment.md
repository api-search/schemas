---
description: Represents a Cloud Composer environment, which is a managed Apache Airflow instance for orchestrating workflows and data pipelines.
layout: schema
name: Google Cloud Composer Environment
properties_list:
- description: The resource name of the environment in the format projects/{project}/locations/{location}/environments/{environment}.
  name: name
  type: string
- description: Configuration parameters for the environment.
  name: config
  type: object
- description: Output only. The UUID of the environment.
  name: uuid
  type: string
- description: The current state of the environment.
  name: state
  type: string
- description: Output only. The time the environment was created.
  name: createTime
  type: string
- description: Output only. The time the environment was last updated.
  name: updateTime
  type: string
- description: User-defined labels for this environment.
  name: labels
  type: object
provider_name: Google Cloud Composer
provider_slug: google-cloud-composer
schema_file: json-schema/google-cloud-composer-environment-schema.json
slug: google-cloud-composer-environment
source_filename: google-cloud-composer-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-composer/refs/heads/main/json-schema/google-cloud-composer-environment-schema.json\",\n  \"title\": \"Google Cloud Composer Environment\",\n  \"description\": \"Represents a Cloud Composer environment, which is a managed Apache Airflow instance for orchestrating workflows and data pipelines.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the environment in the format projects/{project}/locations/{location}/environments/{environment}.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration parameters for the environment.\",\n      \"properties\": {\n        \"gkeCluster\": {\n          \"type\": \"string\",\n          \"description\": \"Output only. The GKE cluster used to run the environment.\"\n \
  \       },\n        \"dagGcsPrefix\": {\n          \"type\": \"string\",\n          \"description\": \"Output only. The Cloud Storage prefix of the DAGs.\"\n        },\n        \"nodeCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of nodes in the GKE cluster.\"\n        },\n        \"softwareConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"imageVersion\": {\n              \"type\": \"string\",\n              \"description\": \"The version of the Composer/Airflow image.\"\n            },\n            \"airflowConfigOverrides\": {\n              \"type\": \"object\",\n              \"additionalProperties\": { \"type\": \"string\" }\n            },\n            \"pypiPackages\": {\n              \"type\": \"object\",\n              \"additionalProperties\": { \"type\": \"string\" }\n            },\n            \"envVariables\": {\n              \"type\": \"object\",\n              \"additionalProperties\": { \"\
  type\": \"string\" }\n            },\n            \"pythonVersion\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"nodeConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"location\": { \"type\": \"string\" },\n            \"machineType\": { \"type\": \"string\" },\n            \"network\": { \"type\": \"string\" },\n            \"subnetwork\": { \"type\": \"string\" },\n            \"diskSizeGb\": { \"type\": \"integer\" },\n            \"serviceAccount\": { \"type\": \"string\" }\n          }\n        },\n        \"environmentSize\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ENVIRONMENT_SIZE_UNSPECIFIED\",\n            \"ENVIRONMENT_SIZE_SMALL\",\n            \"ENVIRONMENT_SIZE_MEDIUM\",\n            \"ENVIRONMENT_SIZE_LARGE\"\n          ]\n        },\n        \"airflowUri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Output\
  \ only. The URI of the Apache Airflow Web UI.\"\n        }\n      }\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The UUID of the environment.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"STATE_UNSPECIFIED\", \"CREATING\", \"RUNNING\", \"UPDATING\", \"DELETING\", \"ERROR\"],\n      \"description\": \"The current state of the environment.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The time the environment was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The time the environment was last updated.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"string\" },\n      \"description\": \"User-defined labels for this environment.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-composer/refs/heads/main/json-schema/google-cloud-composer-environment-schema.json
tags:
- Apache Airflow
- Data Pipelines
- Google Cloud
- Workflow Orchestration
title: Google Cloud Composer Environment
---
