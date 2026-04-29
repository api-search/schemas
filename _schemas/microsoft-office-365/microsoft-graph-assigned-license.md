---
description: Represents a license assigned to a user.
layout: schema
name: AssignedLicense
properties_list:
- description: A collection of unique identifiers for disabled plans.
  name: disabledPlans
  type: array
- description: The unique identifier for the SKU.
  name: skuId
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-assigned-license-schema.json
slug: microsoft-graph-assigned-license
source_filename: microsoft-graph-assigned-license-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssignedLicense\",\n  \"type\": \"object\",\n  \"description\": \"Represents a license assigned to a user.\",\n  \"properties\": {\n    \"disabledPlans\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of unique identifiers for disabled plans.\"\n    },\n    \"skuId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the SKU.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-assigned-license-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: AssignedLicense
---
