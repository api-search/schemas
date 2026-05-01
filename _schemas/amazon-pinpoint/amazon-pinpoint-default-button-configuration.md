---
description: Default button configuration.
layout: schema
name: DefaultButtonConfiguration
properties_list:
- description: ''
  name: BackgroundColor
  type: object
- description: ''
  name: BorderRadius
  type: object
- description: ''
  name: ButtonAction
  type: object
- description: ''
  name: Link
  type: object
- description: ''
  name: Text
  type: object
- description: ''
  name: TextColor
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-default-button-configuration-schema.json
slug: amazon-pinpoint-default-button-configuration
source_filename: amazon-pinpoint-default-button-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-default-button-configuration-schema.json\",\n  \"title\": \"DefaultButtonConfiguration\",\n  \"description\": \"Default button configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BackgroundColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The background color of the button.\"\n        }\n      ]\n    },\n    \"BorderRadius\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The border radius of the button.\"\n        }\n      ]\n    },\n    \"ButtonAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ButtonAction\"\n        },\n        {\n     \
  \     \"description\": \"Action triggered by the button.\"\n        }\n      ]\n    },\n    \"Link\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Button destination.\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Button text.\"\n        }\n      ]\n    },\n    \"TextColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The text color of the button.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ButtonAction\",\n    \"Text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-default-button-configuration-schema.json
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
title: DefaultButtonConfiguration
---
