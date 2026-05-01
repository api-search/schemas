---
description: ListComponentVersionsResponse schema
layout: schema
name: ListComponentVersionsResponse
properties_list:
- description: ''
  name: componentVersions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-list-component-versions-response-schema.json
slug: iot-greengrass-list-component-versions-response
source_filename: iot-greengrass-list-component-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-component-versions-response-schema.json\",\n  \"title\": \"ListComponentVersionsResponse\",\n  \"description\": \"ListComponentVersionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionList\"\n        },\n        {\n          \"description\": \"A list of versions that exist for the component.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextTokenString\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-component-versions-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ListComponentVersionsResponse
---
