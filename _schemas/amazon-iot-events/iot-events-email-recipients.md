---
description: <p>Contains the information of one or more recipients who receive the emails.</p> <important> <p>You must <a href="https://docs.aws.amazon.com/singlesignon/latest/userguide/addusers.html">add the users that receive emails to your AWS SSO store</a>.</p> </important>
layout: schema
name: EmailRecipients
properties_list:
- description: ''
  name: to
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-email-recipients-schema.json
slug: iot-events-email-recipients
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-email-recipients-schema.json\",\n  \"title\": \"EmailRecipients\",\n  \"description\": \"<p>Contains the information of one or more recipients who receive the emails.</p> <important> <p>You must <a href=\\\"https://docs.aws.amazon.com/singlesignon/latest/userguide/addusers.html\\\">add the users that receive emails to your AWS SSO store</a>.</p> </important>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"to\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipientDetails\"\n        },\n        {\n          \"description\": \"Specifies one or more recipients who receive the email.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-email-recipients-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: EmailRecipients
---
