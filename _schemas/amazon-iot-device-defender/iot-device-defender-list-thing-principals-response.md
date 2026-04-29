---
description: The output from the ListThingPrincipals operation.
layout: schema
name: ListThingPrincipalsResponse
properties_list:
- description: ''
  name: principals
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-thing-principals-response-schema.json
slug: iot-device-defender-list-thing-principals-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-thing-principals-response-schema.json\",\n  \"title\": \"ListThingPrincipalsResponse\",\n  \"description\": \"The output from the ListThingPrincipals operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Principals\"\n        },\n        {\n          \"description\": \"The principals associated with the thing.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-thing-principals-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListThingPrincipalsResponse
---
