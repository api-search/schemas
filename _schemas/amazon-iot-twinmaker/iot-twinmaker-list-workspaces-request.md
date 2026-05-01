---
description: ListWorkspacesRequest schema
layout: schema
name: ListWorkspacesRequest
properties_list:
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-workspaces-request-schema.json
slug: iot-twinmaker-list-workspaces-request
source_filename: iot-twinmaker-list-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-workspaces-request-schema.json\",\n  \"title\": \"ListWorkspacesRequest\",\n  \"description\": \"ListWorkspacesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results to return at one time. The default is 25.</p> <p>Valid Range: Minimum value of 1. Maximum value of 250.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-workspaces-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListWorkspacesRequest
---
