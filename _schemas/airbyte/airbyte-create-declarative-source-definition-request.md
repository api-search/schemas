---
description: CreateDeclarativeSourceDefinitionRequest schema from Airbyte API
layout: schema
name: CreateDeclarativeSourceDefinitionRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: manifest
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-create-declarative-source-definition-request-schema.json
slug: airbyte-create-declarative-source-definition-request
source_filename: airbyte-create-declarative-source-definition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-create-declarative-source-definition-request-schema.json\",\n  \"title\": \"CreateDeclarativeSourceDefinitionRequest\",\n  \"description\": \"CreateDeclarativeSourceDefinitionRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"manifest\": {\n      \"$ref\": \"#/components/schemas/DeclarativeManifest\"\n    }\n  },\n  \"required\": [\n    \"workspaceId\",\n    \"name\",\n    \"manifest\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-create-declarative-source-definition-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: CreateDeclarativeSourceDefinitionRequest
---
