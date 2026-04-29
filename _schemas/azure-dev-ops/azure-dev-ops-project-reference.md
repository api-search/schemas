---
description: Reference to an Azure DevOps Project.
layout: schema
name: ProjectReference
properties_list:
- description: Unique immutable identifier of the Azure DevOps Project.
  name: id
  type: string
- description: Name of the Azure DevOps Project.
  name: name
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-project-reference-schema.json
slug: azure-dev-ops-project-reference
source_filename: azure-dev-ops-project-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-project-reference-schema.json\",\n  \"title\": \"ProjectReference\",\n  \"description\": \"Reference to an Azure DevOps Project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique immutable identifier of the Azure DevOps Project.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the Azure DevOps Project.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-project-reference-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: ProjectReference
---
