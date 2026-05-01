---
description: ListTagsForResourceRequest schema
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: resourceARN
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-tags-for-resource-request-schema.json
slug: iot-twinmaker-list-tags-for-resource-request
source_filename: iot-twinmaker-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The ARN of the resource.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results to return at one time. The default is 25.</p> <p>Valid Range: Minimum value of 1. Maximum value of 250.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-tags-for-resource-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListTagsForResourceRequest
---
