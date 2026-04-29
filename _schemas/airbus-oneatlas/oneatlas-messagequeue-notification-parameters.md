---
description: ''
layout: schema
name: MessagequeueNotificationParameters
properties_list:
- description: ''
  name: message
  type: object
- description: Name of the target in message queue service.
  name: target
  type: string
- description: 'URL form is verified. To be done: Endpoint need to be validated.'
  name: url
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-messagequeue-notification-parameters-schema.json
slug: oneatlas-messagequeue-notification-parameters
source_filename: oneatlas-messagequeue-notification-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-messagequeue-notification-parameters-schema.json\",\n  \"title\": \"MessagequeueNotificationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"description\": \"\",\n      \"properties\": {\n        \"header\": {\n          \"description\": \"Message headers transmitted in message queue request.\",\n          \"example\": {\n            \"routing-key\": \"magic-key\"\n          },\n          \"type\": \"object\"\n        },\n        \"properties\": {\n          \"description\": \"Message properties transmitted in message queue request.\",\n          \"example\": {\n            \"correlation-id\": \"magic-id\"\n          },\n          \"type\": \"object\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"target\": {\n      \"description\": \"Name\
  \ of the target in message queue service.\",\n      \"example\": \"magic-queue\",\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"URL form is verified. To be done: Endpoint need to be validated.\",\n      \"example\": \"amqp://user:password@hostname:port/virtualHost\",\n      \"format\": \"url\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-messagequeue-notification-parameters-schema.json
tags:
- Imagery
- Satellites
title: MessagequeueNotificationParameters
---
