---
description: An error returned by the <code>BatchPutProperty</code> action.
layout: schema
name: BatchPutPropertyError
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: entry
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-batch-put-property-error-schema.json
slug: iot-twinmaker-batch-put-property-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-error-schema.json\",\n  \"title\": \"BatchPutPropertyError\",\n  \"description\": \"An error returned by the <code>BatchPutProperty</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message.\"\n        }\n      ]\n    },\n    \"entry\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyValueEntry\"\n        },\n        {\n          \"description\"\
  : \"An object that contains information about errors returned by the <code>BatchPutProperty</code> action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"entry\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-error-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: BatchPutPropertyError
---
