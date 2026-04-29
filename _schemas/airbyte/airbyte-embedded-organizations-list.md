---
description: EmbeddedOrganizationsList schema from Airbyte API
layout: schema
name: EmbeddedOrganizationsList
properties_list:
- description: ''
  name: organizations
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-embedded-organizations-list-schema.json
slug: airbyte-embedded-organizations-list
source_filename: airbyte-embedded-organizations-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-organizations-list-schema.json\",\n  \"title\": \"EmbeddedOrganizationsList\",\n  \"description\": \"EmbeddedOrganizationsList schema from Airbyte API\",\n  \"properties\": {\n    \"organizations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EmbeddedOrganizationListItem\"\n      }\n    }\n  },\n  \"required\": [\n    \"organizations\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-organizations-list-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EmbeddedOrganizationsList
---
