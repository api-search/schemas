---
description: ContactCenterActivity schema from Amazon Pinpoint API
layout: schema
name: ContactCenterActivity
properties_list:
- description: ''
  name: NextActivity
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-contact-center-activity-schema.json
slug: amazon-pinpoint-contact-center-activity
source_filename: amazon-pinpoint-contact-center-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-contact-center-activity-schema.json\",\n  \"title\": \"ContactCenterActivity\",\n  \"description\": \"ContactCenterActivity schema from Amazon Pinpoint API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the next activity to perform after the this activity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-contact-center-activity-schema.json
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
title: ContactCenterActivity
---
