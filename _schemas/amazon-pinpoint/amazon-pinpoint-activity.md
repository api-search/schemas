---
description: Specifies the configuration and other settings for an activity in a journey.
layout: schema
name: Activity
properties_list:
- description: ''
  name: CUSTOM
  type: object
- description: ''
  name: ConditionalSplit
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EMAIL
  type: object
- description: ''
  name: Holdout
  type: object
- description: ''
  name: MultiCondition
  type: object
- description: ''
  name: PUSH
  type: object
- description: ''
  name: RandomSplit
  type: object
- description: ''
  name: SMS
  type: object
- description: ''
  name: Wait
  type: object
- description: ''
  name: ContactCenter
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-activity-schema.json
slug: amazon-pinpoint-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-activity-schema.json\",\n  \"title\": \"Activity\",\n  \"description\": \"Specifies the configuration and other settings for an activity in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CUSTOM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomMessageActivity\"\n        },\n        {\n          \"description\": \"The settings for a custom message activity. This type of activity calls an AWS Lambda function or web hook that sends messages to participants.\"\n        }\n      ]\n    },\n    \"ConditionalSplit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionalSplitActivity\"\n        },\n        {\n          \"description\": \"The settings for a yes/no split activity. This type of activity sends\
  \ participants down one of two paths in a journey, based on conditions that you specify.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the activity.\"\n        }\n      ]\n    },\n    \"EMAIL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailMessageActivity\"\n        },\n        {\n          \"description\": \"The settings for an email activity. This type of activity sends an email message to participants.\"\n        }\n      ]\n    },\n    \"Holdout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HoldoutActivity\"\n        },\n        {\n          \"description\": \"The settings for a holdout activity. This type of activity stops a journey for a specified percentage of participants.\"\n        }\n      ]\n    },\n    \"MultiCondition\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiConditionalSplitActivity\"\n        },\n        {\n          \"description\": \"The settings for a multivariate split activity. This type of activity sends participants down one of as many as five paths (including a default <i>Else</i> path) in a journey, based on conditions that you specify.\"\n        }\n      ]\n    },\n    \"PUSH\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PushMessageActivity\"\n        },\n        {\n          \"description\": \"The settings for a push notification activity. This type of activity sends a push notification to participants.\"\n        }\n      ]\n    },\n    \"RandomSplit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RandomSplitActivity\"\n        },\n        {\n          \"description\": \"The settings for a random split activity. This type of activity randomly sends specified percentages of participants down\
  \ one of as many as five paths in a journey, based on conditions that you specify.\"\n        }\n      ]\n    },\n    \"SMS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMSMessageActivity\"\n        },\n        {\n          \"description\": \"The settings for an SMS activity. This type of activity sends a text message to participants.\"\n        }\n      ]\n    },\n    \"Wait\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WaitActivity\"\n        },\n        {\n          \"description\": \"The settings for a wait activity. This type of activity waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.\"\n        }\n      ]\n    },\n    \"ContactCenter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContactCenterActivity\"\n        },\n        {\n          \"description\": \"The settings for a connect activity. This type\
  \ of activity initiates a contact center call to participants.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-activity-schema.json
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
title: Activity
---
