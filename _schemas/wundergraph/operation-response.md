---
description: A standard response object indicating the success or failure of a platform API operation.
layout: schema
name: WunderGraph Cosmo Operation Response
properties_list:
- description: Whether the operation was successful.
  name: success
  type: boolean
- description: A human-readable response message.
  name: message
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/operation-response.json
slug: operation-response
source_filename: operation-response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/operation-response.json\",\n  \"title\": \"WunderGraph Cosmo Operation Response\",\n  \"description\": \"A standard response object indicating the success or failure of a platform API operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the operation was successful.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable response message.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/operation-response.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Operation Response
---
