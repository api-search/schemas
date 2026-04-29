---
description: A rule that compares an input property value to a threshold value with a comparison operator.
layout: schema
name: SimpleRule
properties_list:
- description: ''
  name: inputProperty
  type: object
- description: ''
  name: comparisonOperator
  type: object
- description: ''
  name: threshold
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-simple-rule-schema.json
slug: iot-events-simple-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-simple-rule-schema.json\",\n  \"title\": \"SimpleRule\",\n  \"description\": \"A rule that compares an input property value to a threshold value with a comparison operator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProperty\"\n        },\n        {\n          \"description\": \"The value on the left side of the comparison operator. You can specify an AWS IoT Events input attribute as an input property.\"\n        }\n      ]\n    },\n    \"comparisonOperator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComparisonOperator\"\n        },\n        {\n          \"description\": \"The comparison operator.\"\n        }\n      ]\n    },\n    \"threshold\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Threshold\"\n        },\n        {\n          \"description\": \"The value on the right side of the comparison operator. You can enter a number or specify an AWS IoT Events input attribute.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputProperty\",\n    \"comparisonOperator\",\n    \"threshold\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-simple-rule-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: SimpleRule
---
