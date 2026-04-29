---
description: Reference to an Azure DevOps Organization.
layout: schema
name: OrganizationReference
properties_list:
- description: Unique immutable identifier for the Azure DevOps Organization.
  name: id
  type: string
- description: Name of the Azure DevOps Organization.
  name: name
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-organization-reference-schema.json
slug: azure-dev-ops-organization-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-organization-reference-schema.json\",\n  \"title\": \"OrganizationReference\",\n  \"description\": \"Reference to an Azure DevOps Organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique immutable identifier for the Azure DevOps Organization.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the Azure DevOps Organization.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-organization-reference-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: OrganizationReference
---
