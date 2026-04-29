---
description: <p/>
layout: schema
name: DataflowEndpointGroupIdResponse
properties_list:
- description: ''
  name: dataflowEndpointGroupId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-dataflow-endpoint-group-id-response-schema.json
slug: ground-station-dataflow-endpoint-group-id-response
source_filename: ground-station-dataflow-endpoint-group-id-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-group-id-response-schema.json\",\n  \"title\": \"DataflowEndpointGroupIdResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataflowEndpointGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a dataflow endpoint group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-dataflow-endpoint-group-id-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DataflowEndpointGroupIdResponse
---
