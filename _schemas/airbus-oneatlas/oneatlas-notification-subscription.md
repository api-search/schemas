---
description: ''
layout: schema
name: NotificationSubscription
properties_list:
- description: ''
  name: channels
  type: array
- description: Object used to filter notifications.
  name: filter
  type: object
- description: ''
  name: id
  type: object
- description: Type of notification
  name: type
  type: string
- description: ''
  name: userId
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-notification-subscription-schema.json
slug: oneatlas-notification-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-notification-subscription-schema.json\",\n  \"title\": \"NotificationSubscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"items\": {\n        \"properties\": {\n          \"parameters\": {\n            \"description\": \"Key/value options of the notification channel. Properties depend on the type of notification channel.\",\n            \"discriminator\": {\n              \"mapping\": {\n                \"email\": \"#/components/schemas/EmailNotificationParameters\",\n                \"messagequeue\": \"#/components/schemas/MessagequeueNotificationParameters\",\n                \"webhook\": \"#/components/schemas/WebhookNotificationParameters\"\n              },\n              \"propertyName\": \"type\"\n            },\n            \"example\": {\n      \
  \        \"addresses\": [\n                \"toto@gmail.com\",\n                \"titi@gmail.com\"\n              ]\n            },\n            \"oneOf\": [\n              {\n                \"$ref\": \"#/components/schemas/EmailNotificationParameters\"\n              },\n              {\n                \"$ref\": \"#/components/schemas/WebhookNotificationParameters\"\n              },\n              {\n                \"$ref\": \"#/components/schemas/MessagequeueNotificationParameters\"\n              }\n            ]\n          },\n          \"type\": {\n            \"description\": \"Type of chanel\",\n            \"enum\": [\n              \"email\",\n              \"messagequeue\",\n              \"webhook\"\n            ],\n            \"example\": \"email\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"type\"\n        ],\n        \"type\": \"object\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\"\n    },\n    \"\
  filter\": {\n      \"description\": \"Object used to filter notifications.\",\n      \"discriminator\": {\n        \"mapping\": {\n          \"activity\": \"#/components/schemas/ActivitySearchOptions\",\n          \"catalogitem\": \"#/components/schemas/SearchOptions\"\n        },\n        \"propertyName\": \"type\"\n      },\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivitySearchOptions\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SearchOptions\"\n        }\n      ]\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    },\n    \"type\": {\n      \"description\": \"Type of notification\",\n      \"enum\": [\n        \"activity\",\n        \"catalogitem\"\n      ],\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The id of the user that is the origin of the notification (extracted\
  \ from the X-Forwarded-User request header)\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channels\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-notification-subscription-schema.json
tags:
- Imagery
- Satellites
title: NotificationSubscription
---
