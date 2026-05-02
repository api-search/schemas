---
description: An Endpoint defines a public-facing URL pattern that the KrakenD gateway exposes to clients, along with its associated backends, encoding, rate limiting, and other configurations.
layout: schema
name: KrakenD Endpoint
properties_list:
- description: The URL pattern the gateway exposes to clients. Must start with a slash.
  name: endpoint
  type: string
- description: The HTTP method this endpoint accepts. Create multiple endpoint entries for different methods.
  name: method
  type: string
- description: The encoding used to render the response to the client.
  name: output_encoding
  type: string
- description: Number of concurrent calls to each backend for this endpoint.
  name: concurrent_calls
  type: integer
- description: Maximum time to wait for the endpoint to complete. E.g., 2s or 2000ms.
  name: timeout
  type: string
- description: Duration for Cache-Control max-age header. E.g., 300s or 5m.
  name: cache_ttl
  type: string
- description: Allowed query string parameters to forward to backends. Use * to forward all.
  name: querystring_params
  type: array
- description: List of client headers forwarded to the backend.
  name: headers_to_pass
  type: array
- description: List of backend definitions this endpoint connects to.
  name: backend
  type: array
- description: Additional component configurations keyed by namespace.
  name: extra_config
  type: object
- description: Recognized query string parameters that can be used in the endpoint.
  name: input_query_strings
  type: array
- description: Recognized headers that can be used in the endpoint.
  name: input_headers
  type: array
provider_name: KrakenD
provider_slug: krakend
schema_file: json-schema/endpoint.json
slug: endpoint
source_filename: endpoint.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/krakend/blob/main/json-schema/endpoint.json\",\n  \"title\": \"KrakenD Endpoint\",\n  \"description\": \"An Endpoint defines a public-facing URL pattern that the KrakenD gateway exposes to clients, along with its associated backends, encoding, rate limiting, and other configurations.\",\n  \"type\": \"object\",\n  \"required\": [\"endpoint\", \"backend\"],\n  \"properties\": {\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The URL pattern the gateway exposes to clients. Must start with a slash.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"],\n      \"description\": \"The HTTP method this endpoint accepts. Create multiple endpoint entries for different methods.\"\n    },\n    \"output_encoding\": {\n      \"type\": \"string\",\n      \"enum\": [\"json\"\
  , \"json-collection\", \"yaml\", \"fast-json\", \"xml\", \"negotiate\", \"string\", \"no-op\"],\n      \"description\": \"The encoding used to render the response to the client.\"\n    },\n    \"concurrent_calls\": {\n      \"type\": \"integer\",\n      \"default\": 1,\n      \"description\": \"Number of concurrent calls to each backend for this endpoint.\"\n    },\n    \"timeout\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum time to wait for the endpoint to complete. E.g., 2s or 2000ms.\"\n    },\n    \"cache_ttl\": {\n      \"type\": \"string\",\n      \"description\": \"Duration for Cache-Control max-age header. E.g., 300s or 5m.\"\n    },\n    \"querystring_params\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Allowed query string parameters to forward to backends. Use * to forward all.\"\n    },\n    \"headers_to_pass\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\":\
  \ \"string\"\n      },\n      \"description\": \"List of client headers forwarded to the backend.\"\n    },\n    \"backend\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"backend.json\"\n      },\n      \"description\": \"List of backend definitions this endpoint connects to.\"\n    },\n    \"extra_config\": {\n      \"type\": \"object\",\n      \"description\": \"Additional component configurations keyed by namespace.\"\n    },\n    \"input_query_strings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Recognized query string parameters that can be used in the endpoint.\"\n    },\n    \"input_headers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Recognized headers that can be used in the endpoint.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/json-schema/endpoint.json
tags:
- Aggregation
- API Gateway
- Go
- Open Source
title: KrakenD Endpoint
---
