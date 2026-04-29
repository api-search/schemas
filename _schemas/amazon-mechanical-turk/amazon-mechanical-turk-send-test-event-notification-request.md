---
description: SendTestEventNotificationRequest schema from Amazon Mechanical Turk API
layout: schema
name: SendTestEventNotificationRequest
properties_list:
- description: ''
  name: Notification
  type: object
- description: ''
  name: TestEventType
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-send-test-event-notification-request-schema.json
slug: amazon-mechanical-turk-send-test-event-notification-request
source_filename: amazon-mechanical-turk-send-test-event-notification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-send-test-event-notification-request-schema.json\",\n  \"title\": \"SendTestEventNotificationRequest\",\n  \"description\": \"SendTestEventNotificationRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationSpecification\"\n        },\n        {\n          \"description\": \" The notification specification to test. This value is identical to the value you would provide to the UpdateNotificationSettings operation when you establish the notification specification for a HIT type. \"\n        }\n      ]\n    },\n    \"TestEventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventType\"\n   \
  \     },\n        {\n          \"description\": \" The event to simulate to test the notification specification. This event is included in the test message even if the notification specification does not include the event type. The notification specification does not filter out the test event. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Notification\",\n    \"TestEventType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-send-test-event-notification-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: SendTestEventNotificationRequest
---
