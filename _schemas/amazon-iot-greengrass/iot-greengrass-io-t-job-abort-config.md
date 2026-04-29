---
description: Contains a list of criteria that define when and how to cancel a configuration deployment.
layout: schema
name: IoTJobAbortConfig
properties_list:
- description: ''
  name: criteriaList
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-io-t-job-abort-config-schema.json
slug: iot-greengrass-io-t-job-abort-config
source_filename: iot-greengrass-io-t-job-abort-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-abort-config-schema.json\",\n  \"title\": \"IoTJobAbortConfig\",\n  \"description\": \"Contains a list of criteria that define when and how to cancel a configuration deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"criteriaList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobAbortCriteriaList\"\n        },\n        {\n          \"description\": \"The list of criteria that define when and how to cancel the configuration deployment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"criteriaList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-abort-config-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: IoTJobAbortConfig
---
