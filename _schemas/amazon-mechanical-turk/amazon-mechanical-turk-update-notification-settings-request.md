---
description: UpdateNotificationSettingsRequest schema from Amazon Mechanical Turk API
layout: schema
name: UpdateNotificationSettingsRequest
properties_list:
- description: ''
  name: HITTypeId
  type: object
- description: ''
  name: Notification
  type: object
- description: ''
  name: Active
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-update-notification-settings-request-schema.json
slug: amazon-mechanical-turk-update-notification-settings-request
source_filename: amazon-mechanical-turk-update-notification-settings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-notification-settings-request-schema.json\",\n  \"title\": \"UpdateNotificationSettingsRequest\",\n  \"description\": \"UpdateNotificationSettingsRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the HIT type whose notification specification is being updated. \"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationSpecification\"\n        },\n        {\n          \"description\": \" The notification specification for the HIT type. \"\n        }\n      ]\n    },\n   \
  \ \"Active\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether notifications are sent for HITs of this HIT type, according to the notification specification. You must specify either the Notification parameter or the Active parameter for the call to UpdateNotificationSettings to succeed. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-notification-settings-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: UpdateNotificationSettingsRequest
---
