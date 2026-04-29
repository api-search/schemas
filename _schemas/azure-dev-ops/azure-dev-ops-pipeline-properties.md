---
description: Custom properties of a Pipeline.
layout: schema
name: PipelineProperties
properties_list:
- description: Configuration used to bootstrap the Pipeline.
  name: bootstrapConfiguration
  type: object
- description: Reference to the Azure DevOps Organization containing the Pipeline.
  name: organization
  type: object
- description: Unique identifier of the Azure Pipeline within the Azure DevOps Project.
  name: pipelineId
  type: integer
- description: Reference to the Azure DevOps Project containing the Pipeline.
  name: project
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-properties-schema.json
slug: azure-dev-ops-pipeline-properties
source_filename: azure-dev-ops-pipeline-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-properties-schema.json\",\n  \"title\": \"PipelineProperties\",\n  \"description\": \"Custom properties of a Pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bootstrapConfiguration\": {\n      \"$ref\": \"#/definitions/BootstrapConfiguration\",\n      \"description\": \"Configuration used to bootstrap the Pipeline.\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/definitions/OrganizationReference\",\n      \"description\": \"Reference to the Azure DevOps Organization containing the Pipeline.\"\n    },\n    \"pipelineId\": {\n      \"description\": \"Unique identifier of the Azure Pipeline within the Azure DevOps Project.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"project\": {\n      \"$ref\": \"#/definitions/ProjectReference\"\
  ,\n      \"description\": \"Reference to the Azure DevOps Project containing the Pipeline.\"\n    }\n  },\n  \"required\": [\n    \"organization\",\n    \"project\",\n    \"bootstrapConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-properties-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineProperties
---
