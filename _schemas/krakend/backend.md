---
description: A Backend defines a target service that a KrakenD endpoint connects to, including the host, URL pattern, encoding, and data manipulation settings.
layout: schema
name: KrakenD Backend
properties_list:
- description: List of backend host URLs. Overrides the service-level host list.
  name: host
  type: array
- description: The URL path to request on the backend. Supports parameter placeholders.
  name: url_pattern
  type: string
- description: The encoding of the backend response.
  name: encoding
  type: string
- description: Service discovery method. Static resolves at startup, DNS resolves per request.
  name: sd
  type: string
- description: HTTP method to use when calling the backend. Defaults to the endpoint method.
  name: method
  type: string
- description: Wraps the backend response under this key name for response merging.
  name: group
  type: string
- description: Extracts a nested object from the backend response using this key.
  name: target
  type: string
- description: Renames backend response fields. Key is original name, value is new name.
  name: mapping
  type: object
- description: Whitelist of fields to include from the backend response.
  name: allow
  type: array
- description: Blacklist of fields to exclude from the backend response.
  name: deny
  type: array
- description: Set to true when the backend response is an array instead of an object.
  name: is_collection
  type: boolean
- description: Additional component configurations keyed by namespace.
  name: extra_config
  type: object
provider_name: KrakenD
provider_slug: krakend
schema_file: json-schema/backend.json
slug: backend
source_filename: backend.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/krakend/blob/main/json-schema/backend.json\",\n  \"title\": \"KrakenD Backend\",\n  \"description\": \"A Backend defines a target service that a KrakenD endpoint connects to, including the host, URL pattern, encoding, and data manipulation settings.\",\n  \"type\": \"object\",\n  \"required\": [\"url_pattern\"],\n  \"properties\": {\n    \"host\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of backend host URLs. Overrides the service-level host list.\"\n    },\n    \"url_pattern\": {\n      \"type\": \"string\",\n      \"description\": \"The URL path to request on the backend. Supports parameter placeholders.\"\n    },\n    \"encoding\": {\n      \"type\": \"string\",\n      \"enum\": [\"json\", \"safejson\", \"xml\", \"rss\", \"string\", \"no-op\"],\n      \"description\": \"The encoding\
  \ of the backend response.\"\n    },\n    \"sd\": {\n      \"type\": \"string\",\n      \"enum\": [\"static\", \"dns\"],\n      \"description\": \"Service discovery method. Static resolves at startup, DNS resolves per request.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"],\n      \"description\": \"HTTP method to use when calling the backend. Defaults to the endpoint method.\"\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"Wraps the backend response under this key name for response merging.\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"Extracts a nested object from the backend response using this key.\"\n    },\n    \"mapping\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Renames backend response fields. Key is original name, value is new name.\"\n\
  \    },\n    \"allow\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Whitelist of fields to include from the backend response.\"\n    },\n    \"deny\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Blacklist of fields to exclude from the backend response.\"\n    },\n    \"is_collection\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Set to true when the backend response is an array instead of an object.\"\n    },\n    \"extra_config\": {\n      \"type\": \"object\",\n      \"description\": \"Additional component configurations keyed by namespace.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/json-schema/backend.json
tags:
- Aggregation
- API Gateway
- Go
- Open Source
title: KrakenD Backend
---
