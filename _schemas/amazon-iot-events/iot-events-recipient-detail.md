---
description: The information that identifies the recipient.
layout: schema
name: RecipientDetail
properties_list:
- description: ''
  name: ssoIdentity
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-recipient-detail-schema.json
slug: iot-events-recipient-detail
source_filename: iot-events-recipient-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-recipient-detail-schema.json\",\n  \"title\": \"RecipientDetail\",\n  \"description\": \"The information that identifies the recipient.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssoIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SSOIdentity\"\n        },\n        {\n          \"description\": \"The AWS Single Sign-On (AWS SSO) authentication information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-recipient-detail-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: RecipientDetail
---
