---
description: CancelServicePipelineDeploymentOutput schema from Amazon Proton API
layout: schema
name: CancelServicePipelineDeploymentOutput
properties_list:
- description: ''
  name: pipeline
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-cancel-service-pipeline-deployment-output-schema.json
slug: amazon-proton-cancel-service-pipeline-deployment-output
source_filename: amazon-proton-cancel-service-pipeline-deployment-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-service-pipeline-deployment-output-schema.json\",\n  \"title\": \"CancelServicePipelineDeploymentOutput\",\n  \"description\": \"CancelServicePipelineDeploymentOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServicePipeline\"\n        },\n        {\n          \"description\": \"The service pipeline detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipeline\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-service-pipeline-deployment-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CancelServicePipelineDeploymentOutput
---
