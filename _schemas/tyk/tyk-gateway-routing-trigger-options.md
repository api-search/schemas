---
description: ''
layout: schema
name: RoutingTriggerOptions
properties_list:
- description: ''
  name: header_matches
  type: object
- description: ''
  name: path_part_matches
  type: object
- description: ''
  name: query_val_matches
  type: object
- description: ''
  name: request_context_matches
  type: object
- description: ''
  name: session_meta_matches
  type: object
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-routing-trigger-options-schema.json
slug: tyk-gateway-routing-trigger-options
source_filename: tyk-gateway-routing-trigger-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoutingTriggerOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"header_matches\": {\n      \"type\": \"object\"\n    },\n    \"path_part_matches\": {\n      \"type\": \"object\"\n    },\n    \"query_val_matches\": {\n      \"type\": \"object\"\n    },\n    \"request_context_matches\": {\n      \"type\": \"object\"\n    },\n    \"session_meta_matches\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-routing-trigger-options-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RoutingTriggerOptions
---
