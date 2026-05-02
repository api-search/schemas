---
description: The root configuration object for a KrakenD API Gateway instance, defining service-level settings, global defaults, and the collection of endpoint definitions.
layout: schema
name: KrakenD Service Configuration
properties_list:
- description: Reference to the KrakenD JSON Schema for IDE autocompletion.
  name: $schema
  type: string
- description: The configuration file version. Must be 3 for KrakenD v2.x.
  name: version
  type: integer
- description: Name of the KrakenD service instance.
  name: name
  type: string
- description: Port on which the gateway listens for incoming requests.
  name: port
  type: integer
- description: Default list of backend hosts used when endpoints do not specify their own.
  name: host
  type: array
- description: Default timeout for all endpoints. E.g., 3s or 3000ms.
  name: timeout
  type: string
- description: Default Cache-Control max-age for all endpoints.
  name: cache_ttl
  type: string
- description: Default output encoding for all endpoints.
  name: output_encoding
  type: string
- description: IP address the service binds to. Empty means all interfaces.
  name: listen_ip
  type: string
- description: Enables the /__debug/ endpoint for request inspection.
  name: debug_endpoint
  type: boolean
- description: Enables the /__echo/ endpoint for request echoing.
  name: echo_endpoint
  type: boolean
- description: Start the gateway only after all async agents are ready.
  name: sequential_start
  type: boolean
- description: The collection of endpoint definitions exposed by the gateway.
  name: endpoints
  type: array
- description: Service-level component configurations keyed by namespace.
  name: extra_config
  type: object
- description: TLS/HTTPS configuration for the gateway.
  name: tls
  type: object
- description: Plugin loader configuration.
  name: plugin
  type: object
- description: Asynchronous agent definitions for consuming from queues and event streams.
  name: async_agent
  type: array
provider_name: KrakenD
provider_slug: krakend
schema_file: json-schema/service-config.json
slug: service-config
source_filename: service-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/krakend/blob/main/json-schema/service-config.json\",\n  \"title\": \"KrakenD Service Configuration\",\n  \"description\": \"The root configuration object for a KrakenD API Gateway instance, defining service-level settings, global defaults, and the collection of endpoint definitions.\",\n  \"type\": \"object\",\n  \"required\": [\"version\", \"endpoints\"],\n  \"properties\": {\n    \"$schema\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the KrakenD JSON Schema for IDE autocompletion.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"enum\": [3],\n      \"description\": \"The configuration file version. Must be 3 for KrakenD v2.x.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the KrakenD service instance.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"default\"\
  : 8080,\n      \"description\": \"Port on which the gateway listens for incoming requests.\"\n    },\n    \"host\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Default list of backend hosts used when endpoints do not specify their own.\"\n    },\n    \"timeout\": {\n      \"type\": \"string\",\n      \"description\": \"Default timeout for all endpoints. E.g., 3s or 3000ms.\"\n    },\n    \"cache_ttl\": {\n      \"type\": \"string\",\n      \"description\": \"Default Cache-Control max-age for all endpoints.\"\n    },\n    \"output_encoding\": {\n      \"type\": \"string\",\n      \"enum\": [\"json\", \"json-collection\", \"yaml\", \"fast-json\", \"xml\", \"negotiate\", \"string\", \"no-op\"],\n      \"description\": \"Default output encoding for all endpoints.\"\n    },\n    \"listen_ip\": {\n      \"type\": \"string\",\n      \"description\": \"IP address the service binds to. Empty means all interfaces.\"\n    },\n\
  \    \"debug_endpoint\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enables the /__debug/ endpoint for request inspection.\"\n    },\n    \"echo_endpoint\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enables the /__echo/ endpoint for request echoing.\"\n    },\n    \"sequential_start\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Start the gateway only after all async agents are ready.\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"endpoint.json\"\n      },\n      \"description\": \"The collection of endpoint definitions exposed by the gateway.\"\n    },\n    \"extra_config\": {\n      \"type\": \"object\",\n      \"description\": \"Service-level component configurations keyed by namespace.\"\n    },\n    \"tls\": {\n      \"$ref\": \"tls.json\",\n      \"description\": \"TLS/HTTPS configuration for the gateway.\"\
  \n    },\n    \"plugin\": {\n      \"$ref\": \"plugin.json\",\n      \"description\": \"Plugin loader configuration.\"\n    },\n    \"async_agent\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"async-agent.json\"\n      },\n      \"description\": \"Asynchronous agent definitions for consuming from queues and event streams.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/json-schema/service-config.json
tags:
- Aggregation
- API Gateway
- Go
- Open Source
title: KrakenD Service Configuration
---
