---
description: Item in a list of <code>DataflowEndpoint</code> groups.
layout: schema
name: DataflowEndpointListItem
properties_list:
- description: ''
  name: dataflowEndpointGroupArn
  type: object
- description: ''
  name: dataflowEndpointGroupId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-dataflow-endpoint-list-item-schema.json
slug: ground-station-dataflow-endpoint-list-item
source_filename: ground-station-dataflow-endpoint-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-list-item-schema.json\",\n  \"title\": \"DataflowEndpointListItem\",\n  \"description\": \"Item in a list of <code>DataflowEndpoint</code> groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataflowEndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointGroupArn\"\n        },\n        {\n          \"description\": \"ARN of a dataflow endpoint group.\"\n        }\n      ]\n    },\n    \"dataflowEndpointGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a dataflow endpoint group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-list-item-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DataflowEndpointListItem
---
