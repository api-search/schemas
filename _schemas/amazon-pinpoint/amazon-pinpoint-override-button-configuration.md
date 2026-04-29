---
description: Override button configuration.
layout: schema
name: OverrideButtonConfiguration
properties_list:
- description: ''
  name: ButtonAction
  type: object
- description: ''
  name: Link
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-override-button-configuration-schema.json
slug: amazon-pinpoint-override-button-configuration
source_filename: amazon-pinpoint-override-button-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-override-button-configuration-schema.json\",\n  \"title\": \"OverrideButtonConfiguration\",\n  \"description\": \"Override button configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ButtonAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ButtonAction\"\n        },\n        {\n          \"description\": \"Action triggered by the button.\"\n        }\n      ]\n    },\n    \"Link\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Button destination.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ButtonAction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-override-button-configuration-schema.json
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
title: OverrideButtonConfiguration
---
