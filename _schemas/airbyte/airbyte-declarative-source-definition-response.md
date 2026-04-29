---
description: DeclarativeSourceDefinitionResponse schema from Airbyte API
layout: schema
name: DeclarativeSourceDefinitionResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: manifest
  type: object
- description: ''
  name: version
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-declarative-source-definition-response-schema.json
slug: airbyte-declarative-source-definition-response
source_filename: airbyte-declarative-source-definition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-declarative-source-definition-response-schema.json\",\n  \"title\": \"DeclarativeSourceDefinitionResponse\",\n  \"description\": \"DeclarativeSourceDefinitionResponse schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"manifest\": {\n      \"$ref\": \"#/components/schemas/DeclarativeManifest\"\n    },\n    \"version\": {\n      \"x-speakeasy-terraform-ignore\": true,\n      \"$ref\": \"#/components/schemas/ManifestVersion\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"manifest\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-declarative-source-definition-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DeclarativeSourceDefinitionResponse
---
