---
description: BatchPutPropertyValuesRequest schema
layout: schema
name: BatchPutPropertyValuesRequest
properties_list:
- description: ''
  name: entries
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-batch-put-property-values-request-schema.json
slug: iot-twinmaker-batch-put-property-values-request
source_filename: iot-twinmaker-batch-put-property-values-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-values-request-schema.json\",\n  \"title\": \"BatchPutPropertyValuesRequest\",\n  \"description\": \"BatchPutPropertyValuesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Entries\"\n        },\n        {\n          \"description\": \"An object that maps strings to the property value entries to set. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-batch-put-property-values-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: BatchPutPropertyValuesRequest
---
