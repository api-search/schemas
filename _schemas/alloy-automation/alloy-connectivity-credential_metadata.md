---
description: Authentication requirements for a connector
layout: schema
name: CredentialMetadata
properties_list:
- description: Connector identifier
  name: connectorId
  type: string
- description: Authentication type required
  name: authType
  type: string
- description: Fields required to create credentials
  name: requiredFields
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-credential_metadata-schema.json
slug: alloy-connectivity-credential_metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-credential_metadata-schema.json\",\n  \"title\": \"CredentialMetadata\",\n  \"type\": \"object\",\n  \"description\": \"Authentication requirements for a connector\",\n  \"properties\": {\n    \"connectorId\": {\n      \"type\": \"string\",\n      \"description\": \"Connector identifier\"\n    },\n    \"authType\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type required\",\n      \"enum\": [\n        \"oauth2\",\n        \"api_key\",\n        \"basic\"\n      ]\n    },\n    \"requiredFields\": {\n      \"type\": \"array\",\n      \"description\": \"Fields required to create credentials\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-credential_metadata-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: CredentialMetadata
---
