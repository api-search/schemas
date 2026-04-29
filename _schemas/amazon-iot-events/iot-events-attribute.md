---
description: The attributes from the JSON payload that are made available by the input. Inputs are derived from messages sent to the AWS IoT Events system using <code>BatchPutMessage</code>. Each such message contains a JSON payload. Those attributes (and their paired values) specified here are available for use in the <code>condition</code> expressions used by detectors.
layout: schema
name: Attribute
properties_list:
- description: ''
  name: jsonPath
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-attribute-schema.json
slug: iot-events-attribute
source_filename: iot-events-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-attribute-schema.json\",\n  \"title\": \"Attribute\",\n  \"description\": \"The attributes from the JSON payload that are made available by the input. Inputs are derived from messages sent to the AWS IoT Events system using <code>BatchPutMessage</code>. Each such message contains a JSON payload. Those attributes (and their paired values) specified here are available for use in the <code>condition</code> expressions used by detectors. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jsonPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeJsonPath\"\n        },\n        {\n          \"description\": \"<p>An expression that specifies an attribute-value pair in a JSON structure. Use this to specify an attribute from the JSON payload that is made\
  \ available by the input. Inputs are derived from messages sent to AWS IoT Events (<code>BatchPutMessage</code>). Each such message contains a JSON payload. The attribute (and its paired value) specified here are available for use in the <code>condition</code> expressions used by detectors. </p> <p>Syntax: <code>&lt;field-name&gt;.&lt;field-name&gt;...</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jsonPath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-attribute-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: Attribute
---
