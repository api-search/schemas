---
description: Information about the dataflow endpoint <code>Config</code>.
layout: schema
name: DataflowEndpointConfig
properties_list:
- description: ''
  name: dataflowEndpointName
  type: object
- description: ''
  name: dataflowEndpointRegion
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-dataflow-endpoint-config-schema.json
slug: ground-station-dataflow-endpoint-config
source_filename: ground-station-dataflow-endpoint-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-config-schema.json\",\n  \"title\": \"DataflowEndpointConfig\",\n  \"description\": \"Information about the dataflow endpoint <code>Config</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataflowEndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Name of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"dataflowEndpointRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Region of a dataflow endpoint.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dataflowEndpointName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-config-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DataflowEndpointConfig
---
