---
description: BatchPutPropertyValuesResponse schema
layout: schema
name: BatchPutPropertyValuesResponse
properties_list:
- description: ''
  name: errorEntries
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-batch-put-property-values-response-schema.json
slug: iot-twinmaker-batch-put-property-values-response
source_filename: iot-twinmaker-batch-put-property-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-values-response-schema.json\",\n  \"title\": \"BatchPutPropertyValuesResponse\",\n  \"description\": \"BatchPutPropertyValuesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorEntries\"\n        },\n        {\n          \"description\": \"Entries that caused errors in the batch put operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorEntries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-values-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: BatchPutPropertyValuesResponse
---
