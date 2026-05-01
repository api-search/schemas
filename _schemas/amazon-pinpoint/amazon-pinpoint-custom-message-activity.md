---
description: The settings for a custom message activity. This type of activity calls an AWS Lambda function or web hook that sends messages to participants.
layout: schema
name: CustomMessageActivity
properties_list:
- description: ''
  name: DeliveryUri
  type: object
- description: ''
  name: EndpointTypes
  type: object
- description: ''
  name: MessageConfig
  type: object
- description: ''
  name: NextActivity
  type: object
- description: ''
  name: TemplateName
  type: object
- description: ''
  name: TemplateVersion
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-custom-message-activity-schema.json
slug: amazon-pinpoint-custom-message-activity
source_filename: amazon-pinpoint-custom-message-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-custom-message-activity-schema.json\",\n  \"title\": \"CustomMessageActivity\",\n  \"description\": \"The settings for a custom message activity. This type of activity calls an AWS Lambda function or web hook that sends messages to participants.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The destination to send the campaign or treatment to. This value can be one of the following:</p> <ul><li><p>The name or Amazon Resource Name (ARN) of an AWS Lambda function to invoke to handle delivery of the campaign or treatment.</p></li> <li><p>The URL for a web application or service that supports HTTPS and can receive the message.\
  \ The URL has to be a full URL, including the HTTPS protocol.</p></li></ul>\"\n        }\n      ]\n    },\n    \"EndpointTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__EndpointTypesElement\"\n        },\n        {\n          \"description\": \"The types of endpoints to send the custom message to. Each valid value maps to a type of channel that you can associate with an endpoint by using the ChannelType property of an endpoint.\"\n        }\n      ]\n    },\n    \"MessageConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneyCustomMessage\"\n        },\n        {\n          \"description\": \"Specifies the message data included in a custom channel message that's sent to participants in a journey.\"\n        }\n      ]\n    },\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier\
  \ for the next activity to perform, after Amazon Pinpoint calls the AWS Lambda function or web hook.\"\n        }\n      ]\n    },\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the custom message template to use for the message. If specified, this value must match the name of an existing message template.\"\n        }\n      ]\n    },\n    \"TemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the version of the message template to use for the message. If specified, this value must match the identifier for an existing template version. To retrieve a list of versions and version identifiers for a template, use the <link  linkend=\\\"templates-template-name-template-type-versions\\\">Template Versions</link> resource.</p> <p>If\
  \ you don't specify a value for this property, Amazon Pinpoint uses the <i>active version</i> of the template. The <i>active version</i> is typically the version of a template that's been most recently reviewed and approved for use, depending on your workflow. It isn't necessarily the latest version of a template.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-custom-message-activity-schema.json
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
title: CustomMessageActivity
---
