---
description: Targeted in-app message campaign.
layout: schema
name: InAppMessageCampaign
properties_list:
- description: ''
  name: CampaignId
  type: object
- description: ''
  name: DailyCap
  type: object
- description: ''
  name: InAppMessage
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: SessionCap
  type: object
- description: ''
  name: TotalCap
  type: object
- description: ''
  name: TreatmentId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-message-campaign-schema.json
slug: amazon-pinpoint-in-app-message-campaign
source_filename: amazon-pinpoint-in-app-message-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-campaign-schema.json\",\n  \"title\": \"InAppMessageCampaign\",\n  \"description\": \"Targeted in-app message campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CampaignId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Campaign id of the corresponding campaign.\"\n        }\n      ]\n    },\n    \"DailyCap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Daily cap which controls the number of times any in-app messages can be shown to the endpoint during a day.\"\n        }\n      ]\n    },\n    \"InAppMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/InAppMessage\"\n        },\n        {\n          \"description\": \"In-app message content with all fields required for rendering an in-app message.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Priority of the in-app message.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppCampaignSchedule\"\n        },\n        {\n          \"description\": \"Schedule of the campaign.\"\n        }\n      ]\n    },\n    \"SessionCap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Session cap which controls the number of times an in-app message can be shown to the endpoint during an application session.\"\n        }\n      ]\n    },\n    \"TotalCap\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Total cap which controls the number of times an in-app message can be shown to the endpoint.\"\n        }\n      ]\n    },\n    \"TreatmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Treatment id of the campaign.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-campaign-schema.json
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
title: InAppMessageCampaign
---
