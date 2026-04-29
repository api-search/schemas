---
description: Specifies the content and "From" address for an email message that's sent to recipients of a campaign.
layout: schema
name: CampaignEmailMessage
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: FromAddress
  type: object
- description: ''
  name: HtmlBody
  type: object
- description: ''
  name: Title
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-email-message-schema.json
slug: amazon-pinpoint-campaign-email-message
source_filename: amazon-pinpoint-campaign-email-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-email-message-schema.json\",\n  \"title\": \"CampaignEmailMessage\",\n  \"description\": \"Specifies the content and \\\"From\\\" address for an email message that's sent to recipients of a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the email for recipients whose email clients don't render HTML content.\"\n        }\n      ]\n    },\n    \"FromAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The verified email address to send the email from. The default address is the FromAddress specified for the\
  \ email channel for the application.\"\n        }\n      ]\n    },\n    \"HtmlBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the email, in HTML format, for recipients whose email clients render HTML content.\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The subject line, or title, of the email.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-email-message-schema.json
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
title: CampaignEmailMessage
---
