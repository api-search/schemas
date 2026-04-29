---
description: Parameters for a custom deployment strategy.
layout: schema
name: CustomDeploymentStrategyParams
properties_list:
- description: The container image that runs the custom deployment logic.
  name: image
  type: string
- description: ''
  name: environment
  type: array
- description: The command to execute in the custom deployer container.
  name: command
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-custom-deployment-strategy-params-schema.json
slug: openshift-rest-custom-deployment-strategy-params
source_filename: openshift-rest-custom-deployment-strategy-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomDeploymentStrategyParams\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for a custom deployment strategy.\",\n  \"properties\": {\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"The container image that runs the custom deployment logic.\"\n    },\n    \"environment\": {\n      \"type\": \"array\"\n    },\n    \"command\": {\n      \"type\": \"array\",\n      \"description\": \"The command to execute in the custom deployer container.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-custom-deployment-strategy-params-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: CustomDeploymentStrategyParams
---
