---
description: Specifies the message configuration for a push notification that's sent to participants in a journey.
layout: schema
name: JourneyPushMessage
properties_list:
- description: ''
  name: TimeToLive
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-push-message-schema.json
slug: amazon-pinpoint-journey-push-message
source_filename: amazon-pinpoint-journey-push-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-push-message-schema.json\",\n  \"title\": \"JourneyPushMessage\",\n  \"description\": \"Specifies the message configuration for a push notification that's sent to participants in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeToLive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The number of seconds that the push notification service should keep the message, if the service is unable to deliver the notification the first time. This value is converted to an expiration value when it's sent to a push-notification service. If this value is 0, the service treats the notification as if it expires immediately and the service doesn't store or try to deliver the notification\
  \ again.</p> <p>This value doesn't apply to messages that are sent through the Amazon Device Messaging (ADM) service.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-push-message-schema.json
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
title: JourneyPushMessage
---
