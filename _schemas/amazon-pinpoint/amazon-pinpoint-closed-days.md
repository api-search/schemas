---
description: The time when journey will stop sending messages.
layout: schema
name: ClosedDays
properties_list:
- description: ''
  name: EMAIL
  type: object
- description: ''
  name: SMS
  type: object
- description: ''
  name: PUSH
  type: object
- description: ''
  name: VOICE
  type: object
- description: ''
  name: CUSTOM
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-closed-days-schema.json
slug: amazon-pinpoint-closed-days
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-closed-days-schema.json\",\n  \"title\": \"ClosedDays\",\n  \"description\": \"The time when journey will stop sending messages.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMAIL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfClosedDaysRules\"\n        },\n        {\n          \"description\": \"Rules for Email Channel.\"\n        }\n      ]\n    },\n    \"SMS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfClosedDaysRules\"\n        },\n        {\n          \"description\": \"Rules for SMS Channel.\"\n        }\n      ]\n    },\n    \"PUSH\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfClosedDaysRules\"\n        },\n        {\n          \"description\": \"Rules\
  \ for Push Channel.\"\n        }\n      ]\n    },\n    \"VOICE\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfClosedDaysRules\"\n        },\n        {\n          \"description\": \"Rules for Voice Channel.\"\n        }\n      ]\n    },\n    \"CUSTOM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfClosedDaysRules\"\n        },\n        {\n          \"description\": \"Rules for Custom Channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-closed-days-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: ClosedDays
---
