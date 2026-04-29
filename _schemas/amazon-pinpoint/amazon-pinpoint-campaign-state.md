---
description: Provides information about the status of a campaign.
layout: schema
name: CampaignState
properties_list:
- description: ''
  name: CampaignStatus
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-state-schema.json
slug: amazon-pinpoint-campaign-state
source_filename: amazon-pinpoint-campaign-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-state-schema.json\",\n  \"title\": \"CampaignState\",\n  \"description\": \"Provides information about the status of a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CampaignStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignStatus\"\n        },\n        {\n          \"description\": \"<p>The current status of the campaign, or the current status of a treatment that belongs to an A/B test campaign.</p> <p>If a campaign uses A/B testing, the campaign has a status of COMPLETED only if all campaign treatments have a status of COMPLETED. If you delete the segment that's associated with a campaign, the campaign fails and has a status of DELETED.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-state-schema.json
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
title: CampaignState
---
