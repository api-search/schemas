---
description: Representation of a pipeline template input parameter value.
layout: schema
name: InputValue
properties_list:
- description: Description of the input parameter value.
  name: displayValue
  type: string
- description: Value of an input parameter.
  name: value
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-input-value-schema.json
slug: azure-dev-ops-input-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-input-value-schema.json\",\n  \"title\": \"InputValue\",\n  \"description\": \"Representation of a pipeline template input parameter value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayValue\": {\n      \"description\": \"Description of the input parameter value.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Value of an input parameter.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-input-value-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: InputValue
---
