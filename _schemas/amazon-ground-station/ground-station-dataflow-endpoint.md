---
description: Information about a dataflow endpoint.
layout: schema
name: DataflowEndpoint
properties_list:
- description: ''
  name: address
  type: object
- description: ''
  name: mtu
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-dataflow-endpoint-schema.json
slug: ground-station-dataflow-endpoint
source_filename: ground-station-dataflow-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-schema.json\",\n  \"title\": \"DataflowEndpoint\",\n  \"description\": \"Information about a dataflow endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SocketAddress\"\n        },\n        {\n          \"description\": \"Socket address of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"mtu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointMtuInteger\"\n        },\n        {\n          \"description\": \"Maximum transmission unit (MTU) size in bytes of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n  \
  \      },\n        {\n          \"description\": \"Name of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointStatus\"\n        },\n        {\n          \"description\": \"Status of a dataflow endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DataflowEndpoint
---
