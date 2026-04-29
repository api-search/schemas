---
description: The attribute payload.
layout: schema
name: AttributePayload
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: merge
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-attribute-payload-schema.json
slug: iot-device-management-attribute-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-attribute-payload-schema.json\",\n  \"title\": \"AttributePayload\",\n  \"description\": \"The attribute payload.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attributes\"\n        },\n        {\n          \"description\": \"<p>A JSON string containing up to three key-value pair in JSON format. For example:</p> <p> <code>{\\\\\\\"attributes\\\\\\\":{\\\\\\\"string1\\\\\\\":\\\\\\\"string2\\\\\\\"}}</code> </p>\"\n        }\n      ]\n    },\n    \"merge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Flag\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the list of attributes provided in the <code>AttributePayload</code>\
  \ is merged with the attributes stored in the registry, instead of overwriting them.</p> <p>To remove an attribute, call <code>UpdateThing</code> with an empty attribute value.</p> <note> <p>The <code>merge</code> attribute is only valid when calling <code>UpdateThing</code> or <code>UpdateThingGroup</code>.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-attribute-payload-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: AttributePayload
---
