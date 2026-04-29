---
description: ListNodesResponse schema from Amazon Panorama
layout: schema
name: ListNodesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Nodes
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-list-nodes-response-schema.json
slug: openapi-list-nodes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-nodes-response-schema.json\",\n  \"title\": \"ListNodesResponse\",\n  \"description\": \"ListNodesResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"Nodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodesList\"\n        },\n        {\n          \"description\": \"A list of nodes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-nodes-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ListNodesResponse
---
