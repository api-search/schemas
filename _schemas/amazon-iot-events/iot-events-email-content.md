---
description: Contains the subject and message of an email.
layout: schema
name: EmailContent
properties_list:
- description: ''
  name: subject
  type: object
- description: ''
  name: additionalMessage
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-email-content-schema.json
slug: iot-events-email-content
source_filename: iot-events-email-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-email-content-schema.json\",\n  \"title\": \"EmailContent\",\n  \"description\": \"Contains the subject and message of an email.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailSubject\"\n        },\n        {\n          \"description\": \"The subject of the email.\"\n        }\n      ]\n    },\n    \"additionalMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationAdditionalMessage\"\n        },\n        {\n          \"description\": \"The message that you want to send. The message can be up to 200 characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-email-content-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: EmailContent
---
