---
description: Specifies the settings for events that cause a campaign to be sent.
layout: schema
name: CampaignEventFilter
properties_list:
- description: ''
  name: Dimensions
  type: object
- description: ''
  name: FilterType
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-event-filter-schema.json
slug: amazon-pinpoint-campaign-event-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-event-filter-schema.json\",\n  \"title\": \"CampaignEventFilter\",\n  \"description\": \"Specifies the settings for events that cause a campaign to be sent.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventDimensions\"\n        },\n        {\n          \"description\": \"The dimension settings of the event filter for the campaign.\"\n        }\n      ]\n    },\n    \"FilterType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterType\"\n        },\n        {\n          \"description\": \"The type of event that causes the campaign to be sent. Valid values are: SYSTEM, sends the campaign when a system event occurs; and, ENDPOINT, sends the campaign\
  \ when an endpoint event (<link  linkend=\\\"apps-application-id-events\\\">Events</link> resource) occurs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FilterType\",\n    \"Dimensions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-event-filter-schema.json
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
title: CampaignEventFilter
---
