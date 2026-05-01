---
description: The time when journey allow to send messages. QuietTime should be configured first and SendingSchedule should be set to true.
layout: schema
name: OpenHours
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
schema_file: json-schema/amazon-pinpoint-open-hours-schema.json
slug: amazon-pinpoint-open-hours
source_filename: amazon-pinpoint-open-hours-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-open-hours-schema.json\",\n  \"title\": \"OpenHours\",\n  \"description\": \"The time when journey allow to send messages. QuietTime should be configured first and SendingSchedule should be set to true.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMAIL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOfOpenHoursRules\"\n        },\n        {\n          \"description\": \"Rules for Email Channel.\"\n        }\n      ]\n    },\n    \"SMS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOfOpenHoursRules\"\n        },\n        {\n          \"description\": \"Rules for SMS Channel.\"\n        }\n      ]\n    },\n    \"PUSH\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOfOpenHoursRules\"\
  \n        },\n        {\n          \"description\": \"Rules for Push Channel.\"\n        }\n      ]\n    },\n    \"VOICE\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOfOpenHoursRules\"\n        },\n        {\n          \"description\": \"Rules for Voice Channel.\"\n        }\n      ]\n    },\n    \"CUSTOM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOfOpenHoursRules\"\n        },\n        {\n          \"description\": \"Rules for Custom Channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-open-hours-schema.json
tags:
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
title: OpenHours
---
