---
description: CancelServicePipelineDeploymentInput schema from Amazon Proton API
layout: schema
name: CancelServicePipelineDeploymentInput
properties_list:
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-cancel-service-pipeline-deployment-input-schema.json
slug: amazon-proton-cancel-service-pipeline-deployment-input
source_filename: amazon-proton-cancel-service-pipeline-deployment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-service-pipeline-deployment-input-schema.json\",\n  \"title\": \"CancelServicePipelineDeploymentInput\",\n  \"description\": \"CancelServicePipelineDeploymentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service with the service pipeline deployment to cancel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-service-pipeline-deployment-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CancelServicePipelineDeploymentInput
---
