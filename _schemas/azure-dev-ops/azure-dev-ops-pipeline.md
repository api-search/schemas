---
description: Azure DevOps Pipeline used to configure Continuous Integration (CI) & Continuous Delivery (CD) for Azure resources.
layout: schema
name: Pipeline
properties_list:
- description: Custom properties of the Pipeline.
  name: properties
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-schema.json
slug: azure-dev-ops-pipeline
source_filename: azure-dev-ops-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-schema.json\",\n  \"title\": \"Pipeline\",\n  \"description\": \"Azure DevOps Pipeline used to configure Continuous Integration (CI) & Continuous Delivery (CD) for Azure resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/PipelineProperties\",\n      \"description\": \"Custom properties of the Pipeline.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: Pipeline
---
