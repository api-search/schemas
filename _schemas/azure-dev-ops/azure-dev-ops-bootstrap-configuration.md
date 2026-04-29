---
description: Configuration used to bootstrap a Pipeline.
layout: schema
name: BootstrapConfiguration
properties_list:
- description: Repository containing the source code for the pipeline.
  name: repository
  type: object
- description: Template used to bootstrap the pipeline.
  name: template
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-bootstrap-configuration-schema.json
slug: azure-dev-ops-bootstrap-configuration
source_filename: azure-dev-ops-bootstrap-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-bootstrap-configuration-schema.json\",\n  \"title\": \"BootstrapConfiguration\",\n  \"description\": \"Configuration used to bootstrap a Pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"$ref\": \"#/definitions/CodeRepository\",\n      \"description\": \"Repository containing the source code for the pipeline.\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/PipelineTemplate\",\n      \"description\": \"Template used to bootstrap the pipeline.\"\n    }\n  },\n  \"required\": [\n    \"template\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-bootstrap-configuration-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: BootstrapConfiguration
---
