---
description: Request payload used to update an existing Azure Pipeline.
layout: schema
name: PipelineUpdateParameters
properties_list:
- description: Dictionary of key-value pairs to be set as tags on the Azure Pipeline. This will overwrite any existing tags.
  name: tags
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-update-parameters-schema.json
slug: azure-dev-ops-pipeline-update-parameters
source_filename: azure-dev-ops-pipeline-update-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-update-parameters-schema.json\",\n  \"title\": \"PipelineUpdateParameters\",\n  \"description\": \"Request payload used to update an existing Azure Pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Dictionary of key-value pairs to be set as tags on the Azure Pipeline. This will overwrite any existing tags.\",\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-update-parameters-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineUpdateParameters
---
