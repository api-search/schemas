---
description: UpdateServicePipelineOutput schema from Amazon Proton API
layout: schema
name: UpdateServicePipelineOutput
properties_list:
- description: ''
  name: pipeline
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-pipeline-output-schema.json
slug: amazon-proton-update-service-pipeline-output
source_filename: amazon-proton-update-service-pipeline-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-pipeline-output-schema.json\",\n  \"title\": \"UpdateServicePipelineOutput\",\n  \"description\": \"UpdateServicePipelineOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServicePipeline\"\n        },\n        {\n          \"description\": \"The pipeline details that are returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipeline\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-pipeline-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServicePipelineOutput
---
