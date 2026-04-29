---
description: CancelEnvironmentDeploymentInput schema from Amazon Proton API
layout: schema
name: CancelEnvironmentDeploymentInput
properties_list:
- description: ''
  name: environmentName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-cancel-environment-deployment-input-schema.json
slug: amazon-proton-cancel-environment-deployment-input
source_filename: amazon-proton-cancel-environment-deployment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-environment-deployment-input-schema.json\",\n  \"title\": \"CancelEnvironmentDeploymentInput\",\n  \"description\": \"CancelEnvironmentDeploymentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment with the deployment to cancel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-environment-deployment-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CancelEnvironmentDeploymentInput
---
