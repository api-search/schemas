---
description: ProviderMetadataInfo schema from Ampersand API
layout: schema
name: ProviderMetadataInfo
properties_list:
- description: The value of the metadata field
  name: value
  type: string
- description: The source of the metadata field
  name: source
  type: string
- description: The human-readable name for the field
  name: displayName
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-provider-metadata-info-schema.json
slug: ampersand-api-provider-metadata-info
source_filename: ampersand-api-provider-metadata-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-provider-metadata-info-schema.json\",\n  \"title\": \"ProviderMetadataInfo\",\n  \"description\": \"ProviderMetadataInfo schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the metadata field\",\n      \"example\": \"1234567890\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the metadata field\",\n      \"enum\": [\n        \"input\",\n        \"token\",\n        \"provider\"\n      ],\n      \"example\": \"input\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name for the field\",\n      \"example\": \"Account ID\"\n    }\n  },\n  \"required\": [\n    \"value\",\n    \"source\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-provider-metadata-info-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ProviderMetadataInfo
---
