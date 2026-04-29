---
description: The NotificationSpecification data structure describes a HIT event notification for a HIT type.
layout: schema
name: NotificationSpecification
properties_list:
- description: ''
  name: Destination
  type: object
- description: ''
  name: Transport
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: EventTypes
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-notification-specification-schema.json
slug: amazon-mechanical-turk-notification-specification
source_filename: amazon-mechanical-turk-notification-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-notification-specification-schema.json\",\n  \"title\": \"NotificationSpecification\",\n  \"description\": \"The NotificationSpecification data structure describes a HIT event notification for a HIT type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> The target for notification messages. The Destination\\u2019s format is determined by the specified Transport: </p> <ul> <li> <p>When Transport is Email, the Destination is your email address.</p> </li> <li> <p>When Transport is SQS, the Destination is your queue URL.</p> </li> <li> <p>When Transport is SNS, the Destination is the ARN of your topic.</p> </li> </ul>\"\
  \n        }\n      ]\n    },\n    \"Transport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTransport\"\n        },\n        {\n          \"description\": \" The method Amazon Mechanical Turk uses to send the notification. Valid Values: Email | SQS | SNS. \"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The version of the Notification API to use. Valid value is 2006-05-05.\"\n        }\n      ]\n    },\n    \"EventTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventTypeList\"\n        },\n        {\n          \"description\": \" The list of events that should cause notifications to be sent. Valid Values: AssignmentAccepted | AssignmentAbandoned | AssignmentReturned | AssignmentSubmitted | AssignmentRejected | AssignmentApproved | HITCreated | HITExtended | HITDisposed\
  \ | HITReviewable | HITExpired | Ping. The Ping event is only valid for the SendTestEventNotification operation. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\",\n    \"Transport\",\n    \"Version\",\n    \"EventTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-notification-specification-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: NotificationSpecification
---
