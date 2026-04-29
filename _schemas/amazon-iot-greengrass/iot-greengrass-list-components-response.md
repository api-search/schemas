---
description: ListComponentsResponse schema
layout: schema
name: ListComponentsResponse
properties_list:
- description: ''
  name: components
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-list-components-response-schema.json
slug: iot-greengrass-list-components-response
source_filename: iot-greengrass-list-components-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-components-response-schema.json\",\n  \"title\": \"ListComponentsResponse\",\n  \"description\": \"ListComponentsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentList\"\n        },\n        {\n          \"description\": \"A list that summarizes each component.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextTokenString\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-components-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ListComponentsResponse
---
