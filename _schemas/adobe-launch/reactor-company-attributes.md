---
description: ''
layout: schema
name: CompanyAttributes
properties_list:
- description: The name of the company.
  name: name
  type: string
- description: The Adobe organization ID.
  name: org_id
  type: string
- description: A unique token for the company.
  name: token
  type: string
- description: When the company was created.
  name: created_at
  type: string
- description: When the company was last updated.
  name: updated_at
  type: string
- description: Whether Customer Journey Management is enabled.
  name: cjm_enabled
  type: boolean
- description: Whether Edge capabilities are enabled.
  name: edge_enabled
  type: boolean
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-company-attributes-schema.json
slug: reactor-company-attributes
source_filename: reactor-company-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompanyAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the company.\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Adobe organization ID.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"A unique token for the company.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the company was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the company was last updated.\"\n    },\n    \"cjm_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Customer Journey Management is enabled.\"\n    },\n    \"edge_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Edge capabilities are enabled.\"\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-company-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: CompanyAttributes
---
