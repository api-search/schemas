---
description: Specifies the settings for a push notification activity in a journey. This type of activity sends a push notification to participants.
layout: schema
name: PushMessageActivity
properties_list:
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
schema_file: json-schema/amazon-pinpoint-push-message-activity-schema.json
slug: amazon-pinpoint-push-message-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-push-message-activity-schema.json\",\n  \"title\": \"PushMessageActivity\",\n  \"description\": \"Specifies the settings for a push notification activity in a journey. This type of activity sends a push notification to participants.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneyPushMessage\"\n        },\n        {\n          \"description\": \"Specifies the time to live (TTL) value for push notifications that are sent to participants in a journey.\"\n        }\n      ]\n    },\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the next activity\
  \ to perform, after the message is sent.\"\n        }\n      ]\n    },\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the push notification template to use for the message. If specified, this value must match the name of an existing message template.\"\n        }\n      ]\n    },\n    \"TemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the version of the push notification template to use for the message. If specified, this value must match the identifier for an existing template version. To retrieve a list of versions and version identifiers for a template, use the <link  linkend=\\\"templates-template-name-template-type-versions\\\">Template Versions</link> resource.</p> <p>If you don't specify a value for this property,\
  \ Amazon Pinpoint uses the <i>active version</i> of the template. The <i>active version</i> is typically the version of a template that's been most recently reviewed and approved for use, depending on your workflow. It isn't necessarily the latest version of a template.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-push-message-activity-schema.json
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
title: PushMessageActivity
---
