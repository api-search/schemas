---
description: RecipientDetails schema
layout: schema
name: RecipientDetails
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-recipient-details-schema.json
slug: iot-events-recipient-details
source_filename: iot-events-recipient-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-recipient-details-schema.json\",\n  \"title\": \"RecipientDetails\",\n  \"description\": \"RecipientDetails schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ssoIdentity\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SSOIdentity\"\n          },\n          {\n            \"description\": \"The AWS Single Sign-On (AWS SSO) authentication information.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The information that identifies the recipient.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-recipient-details-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: RecipientDetails
---
