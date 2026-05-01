---
description: Schedule of the campaign.
layout: schema
name: InAppCampaignSchedule
properties_list:
- description: ''
  name: EndDate
  type: object
- description: ''
  name: EventFilter
  type: object
- description: ''
  name: QuietTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-campaign-schedule-schema.json
slug: amazon-pinpoint-in-app-campaign-schedule
source_filename: amazon-pinpoint-in-app-campaign-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-campaign-schedule-schema.json\",\n  \"title\": \"InAppCampaignSchedule\",\n  \"description\": \"Schedule of the campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The scheduled time after which the in-app message should not be shown. Timestamp is in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"EventFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignEventFilter\"\n        },\n        {\n          \"description\": \"The event filter the SDK has to use to show the in-app message in the application.\"\n        }\n      ]\n    },\n    \"QuietTime\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/QuietTime\"\n        },\n        {\n          \"description\": \"Time during which the in-app message should not be shown to the user.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-campaign-schedule-schema.json
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
title: InAppCampaignSchedule
---
