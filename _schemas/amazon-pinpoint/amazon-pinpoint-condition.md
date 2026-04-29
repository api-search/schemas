---
description: Specifies the conditions to evaluate for an activity in a journey, and how to evaluate those conditions.
layout: schema
name: Condition
properties_list:
- description: ''
  name: Conditions
  type: object
- description: ''
  name: Operator
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-condition-schema.json
slug: amazon-pinpoint-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-condition-schema.json\",\n  \"title\": \"Condition\",\n  \"description\": \"Specifies the conditions to evaluate for an activity in a journey, and how to evaluate those conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Conditions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfSimpleCondition\"\n        },\n        {\n          \"description\": \"The conditions to evaluate for the activity.\"\n        }\n      ]\n    },\n    \"Operator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Operator\"\n        },\n        {\n          \"description\": \"Specifies how to handle multiple conditions for the activity. For example, if you specify two conditions for an activity, whether both or only one of the conditions\
  \ must be met for the activity to be performed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-condition-schema.json
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
title: Condition
---
