---
description: <p/>
layout: schema
name: ListDataflowEndpointGroupsResponse
properties_list:
- description: ''
  name: dataflowEndpointGroupList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-list-dataflow-endpoint-groups-response-schema.json
slug: ground-station-list-dataflow-endpoint-groups-response
source_filename: ground-station-list-dataflow-endpoint-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-dataflow-endpoint-groups-response-schema.json\",\n  \"title\": \"ListDataflowEndpointGroupsResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataflowEndpointGroupList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointGroupList\"\n        },\n        {\n          \"description\": \"A list of dataflow endpoint groups.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Next token returned in the response of a previous <code>ListDataflowEndpointGroups</code> call. Used to get the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-dataflow-endpoint-groups-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ListDataflowEndpointGroupsResponse
---
