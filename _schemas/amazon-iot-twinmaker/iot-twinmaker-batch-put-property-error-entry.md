---
description: An object that contains information about errors returned by the <code>BatchPutProperty</code> action.
layout: schema
name: BatchPutPropertyErrorEntry
properties_list:
- description: ''
  name: errors
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-batch-put-property-error-entry-schema.json
slug: iot-twinmaker-batch-put-property-error-entry
source_filename: iot-twinmaker-batch-put-property-error-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-error-entry-schema.json\",\n  \"title\": \"BatchPutPropertyErrorEntry\",\n  \"description\": \"An object that contains information about errors returned by the <code>BatchPutProperty</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Errors\"\n        },\n        {\n          \"description\": \"A list of objects that contain information about errors returned by the <code>BatchPutProperty</code> action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-error-entry-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: BatchPutPropertyErrorEntry
---
