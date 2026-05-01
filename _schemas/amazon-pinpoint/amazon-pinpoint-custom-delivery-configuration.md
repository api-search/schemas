---
description: Specifies the delivery configuration settings for sending a campaign or campaign treatment through a custom channel. This object is required if you use the CampaignCustomMessage object to define the message to send for the campaign or campaign treatment.
layout: schema
name: CustomDeliveryConfiguration
properties_list:
- description: ''
  name: DeliveryUri
  type: object
- description: ''
  name: EndpointTypes
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-custom-delivery-configuration-schema.json
slug: amazon-pinpoint-custom-delivery-configuration
source_filename: amazon-pinpoint-custom-delivery-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-custom-delivery-configuration-schema.json\",\n  \"title\": \"CustomDeliveryConfiguration\",\n  \"description\": \"Specifies the delivery configuration settings for sending a campaign or campaign treatment through a custom channel. This object is required if you use the CampaignCustomMessage object to define the message to send for the campaign or campaign treatment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The destination to send the campaign or treatment to. This value can be one of the following:</p> <ul><li><p>The name or Amazon Resource Name (ARN) of an AWS Lambda function to invoke to handle delivery of the campaign\
  \ or treatment.</p></li> <li><p>The URL for a web application or service that supports HTTPS and can receive the message. The URL has to be a full URL, including the HTTPS protocol.</p></li></ul> \"\n        }\n      ]\n    },\n    \"EndpointTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__EndpointTypesElement\"\n        },\n        {\n          \"description\": \"The types of endpoints to send the campaign or treatment to. Each valid value maps to a type of channel that you can associate with an endpoint by using the ChannelType property of an endpoint.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeliveryUri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-custom-delivery-configuration-schema.json
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
title: CustomDeliveryConfiguration
---
