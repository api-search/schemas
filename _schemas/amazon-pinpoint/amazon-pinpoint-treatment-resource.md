---
description: Specifies the settings for a campaign treatment. A <i>treatment</i> is a variation of a campaign that's used for A/B testing of a campaign.
layout: schema
name: TreatmentResource
properties_list:
- description: ''
  name: CustomDeliveryConfiguration
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: MessageConfiguration
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: SizePercent
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: TemplateConfiguration
  type: object
- description: ''
  name: TreatmentDescription
  type: object
- description: ''
  name: TreatmentName
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-treatment-resource-schema.json
slug: amazon-pinpoint-treatment-resource
source_filename: amazon-pinpoint-treatment-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-treatment-resource-schema.json\",\n  \"title\": \"TreatmentResource\",\n  \"description\": \"Specifies the settings for a campaign treatment. A <i>treatment</i> is a variation of a campaign that's used for A/B testing of a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The delivery configuration settings for sending the treatment through a custom channel. This object is required if the MessageConfiguration object for the treatment specifies a CustomMessage object.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The unique identifier for the treatment.\"\n        }\n      ]\n    },\n    \"MessageConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageConfiguration\"\n        },\n        {\n          \"description\": \"The message configuration settings for the treatment.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Schedule\"\n        },\n        {\n          \"description\": \"The schedule settings for the treatment.\"\n        }\n      ]\n    },\n    \"SizePercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The allocated percentage of users (segment members) that the treatment is sent to.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignState\"\
  \n        },\n        {\n          \"description\": \"The current status of the treatment.\"\n        }\n      ]\n    },\n    \"TemplateConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateConfiguration\"\n        },\n        {\n          \"description\": \"The message template to use for the treatment.\"\n        }\n      ]\n    },\n    \"TreatmentDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the treatment.\"\n        }\n      ]\n    },\n    \"TreatmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the treatment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"SizePercent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-treatment-resource-schema.json
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
title: TreatmentResource
---
