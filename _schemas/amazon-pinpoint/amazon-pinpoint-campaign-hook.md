---
description: Specifies settings for invoking an AWS Lambda function that customizes a segment for a campaign.
layout: schema
name: CampaignHook
properties_list:
- description: ''
  name: LambdaFunctionName
  type: object
- description: ''
  name: Mode
  type: object
- description: ''
  name: WebUrl
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-hook-schema.json
slug: amazon-pinpoint-campaign-hook
source_filename: amazon-pinpoint-campaign-hook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-hook-schema.json\",\n  \"title\": \"CampaignHook\",\n  \"description\": \"Specifies settings for invoking an AWS Lambda function that customizes a segment for a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LambdaFunctionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name or Amazon Resource Name (ARN) of the AWS Lambda function that Amazon Pinpoint invokes to customize a segment for a campaign.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mode\"\n        },\n        {\n          \"description\": \"<p>The mode that Amazon Pinpoint uses to invoke the AWS Lambda function. Possible\
  \ values are:</p> <ul><li><p>FILTER - Invoke the function to customize the segment that's used by a campaign.</p></li> <li><p>DELIVERY - (Deprecated) Previously, invoked the function to send a campaign through a custom channel. This functionality is not supported anymore. To send a campaign through a custom channel, use the CustomDeliveryConfiguration and CampaignCustomMessage objects of the campaign.</p></li></ul>\"\n        }\n      ]\n    },\n    \"WebUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \" <p>The web URL that Amazon Pinpoint calls to invoke the AWS Lambda function over HTTPS.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-hook-schema.json
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
title: CampaignHook
---
