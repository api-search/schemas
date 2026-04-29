---
description: Represents a license assigned to a user
layout: schema
name: AssignedLicense
properties_list:
- description: Collection of unique identifiers for disabled service plans
  name: disabledPlans
  type: array
- description: Unique identifier for the SKU
  name: skuId
  type: string
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-assigned-license-schema.json
slug: microsoft-entra-graph-identity-assigned-license
source_filename: microsoft-entra-graph-identity-assigned-license-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssignedLicense\",\n  \"type\": \"object\",\n  \"description\": \"Represents a license assigned to a user\",\n  \"properties\": {\n    \"disabledPlans\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of unique identifiers for disabled service plans\"\n    },\n    \"skuId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the SKU\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-assigned-license-schema.json
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
title: AssignedLicense
---
