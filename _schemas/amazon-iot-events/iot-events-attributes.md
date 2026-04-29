---
description: Attributes schema
layout: schema
name: Attributes
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-attributes-schema.json
slug: iot-events-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-attributes-schema.json\",\n  \"title\": \"Attributes\",\n  \"description\": \"Attributes schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"jsonPath\"\n    ],\n    \"properties\": {\n      \"jsonPath\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AttributeJsonPath\"\n          },\n          {\n            \"description\": \"<p>An expression that specifies an attribute-value pair in a JSON structure. Use this to specify an attribute from the JSON payload that is made available by the input. Inputs are derived from messages sent to AWS IoT Events (<code>BatchPutMessage</code>). Each such message contains a JSON payload. The attribute (and its paired value) specified here are available for use in the\
  \ <code>condition</code> expressions used by detectors. </p> <p>Syntax: <code>&lt;field-name&gt;.&lt;field-name&gt;...</code> </p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The attributes from the JSON payload that are made available by the input. Inputs are derived from messages sent to the AWS IoT Events system using <code>BatchPutMessage</code>. Each such message contains a JSON payload. Those attributes (and their paired values) specified here are available for use in the <code>condition</code> expressions used by detectors. \"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-attributes-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: Attributes
---
