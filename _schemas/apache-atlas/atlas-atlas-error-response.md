---
description: Error response from the Apache Atlas REST API.
layout: schema
name: AtlasErrorResponse
properties_list:
- description: Unique request identifier for tracing.
  name: requestId
  type: string
- description: Atlas error code.
  name: errorCode
  type: string
- description: Human-readable error message.
  name: errorMessage
  type: string
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-error-response-schema.json
slug: atlas-atlas-error-response
source_filename: atlas-atlas-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-error-response-schema.json\",\n  \"title\": \"AtlasErrorResponse\",\n  \"description\": \"Error response from the Apache Atlas REST API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request identifier for tracing.\",\n      \"example\": \"req-123456\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Atlas error code.\",\n      \"example\": \"ATLAS-400-00-004\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\",\n      \"example\": \"Entity not found for GUID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-error-response-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasErrorResponse
---
