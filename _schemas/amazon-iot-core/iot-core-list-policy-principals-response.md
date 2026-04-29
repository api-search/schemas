---
description: The output from the ListPolicyPrincipals operation.
layout: schema
name: ListPolicyPrincipalsResponse
properties_list:
- description: ''
  name: principals
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-policy-principals-response-schema.json
slug: iot-core-list-policy-principals-response
source_filename: iot-core-list-policy-principals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-policy-principals-response-schema.json\",\n  \"title\": \"ListPolicyPrincipalsResponse\",\n  \"description\": \"The output from the ListPolicyPrincipals operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Principals\"\n        },\n        {\n          \"description\": \"The descriptions of the principals.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The marker for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-policy-principals-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListPolicyPrincipalsResponse
---
