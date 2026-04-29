---
description: <p>Information needed to configure the payload.</p> <p>By default, AWS IoT Events generates a standard payload in JSON for any action. This action payload contains all attribute-value pairs that have the information about the detector model instance and the event triggered the action. To configure the action payload, you can use <code>contentExpression</code>.</p>
layout: schema
name: Payload
properties_list:
- description: ''
  name: contentExpression
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-payload-schema.json
slug: iot-events-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-payload-schema.json\",\n  \"title\": \"Payload\",\n  \"description\": \"<p>Information needed to configure the payload.</p> <p>By default, AWS IoT Events generates a standard payload in JSON for any action. This action payload contains all attribute-value pairs that have the information about the detector model instance and the event triggered the action. To configure the action payload, you can use <code>contentExpression</code>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContentExpression\"\n        },\n        {\n          \"description\": \"The content of the payload. You can use a string expression that includes quoted strings (<code>'&lt;string&gt;'</code>), variables (<code>$variable.&lt;variable-name&gt;</code>),\
  \ input values (<code>$input.&lt;input-name&gt;.&lt;path-to-datum&gt;</code>), string concatenations, and quoted strings that contain <code>${}</code> as the content. The recommended maximum size of a content expression is 1 KB.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PayloadType\"\n        },\n        {\n          \"description\": \"The value of the payload type can be either <code>STRING</code> or <code>JSON</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"contentExpression\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-payload-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: Payload
---
