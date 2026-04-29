---
description: Contains the configuration information of SMS notifications.
layout: schema
name: SMSConfiguration
properties_list:
- description: ''
  name: senderId
  type: object
- description: ''
  name: additionalMessage
  type: object
- description: ''
  name: recipients
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-s-m-s-configuration-schema.json
slug: iot-events-s-m-s-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-s-m-s-configuration-schema.json\",\n  \"title\": \"SMSConfiguration\",\n  \"description\": \"Contains the configuration information of SMS notifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"senderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMSSenderId\"\n        },\n        {\n          \"description\": \"The sender ID.\"\n        }\n      ]\n    },\n    \"additionalMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationAdditionalMessage\"\n        },\n        {\n          \"description\": \"The message that you want to send. The message can be up to 200 characters.\"\n        }\n      ]\n    },\n    \"recipients\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipientDetails\"\
  \n        },\n        {\n          \"description\": \"<p>Specifies one or more recipients who receive the message.</p> <important> <p>You must <a href=\\\"https://docs.aws.amazon.com/singlesignon/latest/userguide/addusers.html\\\">add the users that receive SMS messages to your AWS SSO store</a>.</p> </important>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"recipients\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-s-m-s-configuration-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: SMSConfiguration
---
