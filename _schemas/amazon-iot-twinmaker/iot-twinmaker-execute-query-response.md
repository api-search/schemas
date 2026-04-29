---
description: ExecuteQueryResponse schema
layout: schema
name: ExecuteQueryResponse
properties_list:
- description: ''
  name: columnDescriptions
  type: object
- description: ''
  name: rows
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-execute-query-response-schema.json
slug: iot-twinmaker-execute-query-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-execute-query-response-schema.json\",\n  \"title\": \"ExecuteQueryResponse\",\n  \"description\": \"ExecuteQueryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"columnDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnDescriptions\"\n        },\n        {\n          \"description\": \"A list of ColumnDescription objects.\"\n        }\n      ]\n    },\n    \"rows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rows\"\n        },\n        {\n          \"description\": \"Represents a single row in the query results.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n        \
  \  \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-execute-query-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ExecuteQueryResponse
---
