---
description: ''
layout: schema
name: WebhookNotificationParameters
properties_list:
- description: 'URL form is verified. To be done: Endpoint need to be validated.'
  name: url
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-webhook-notification-parameters-schema.json
slug: oneatlas-webhook-notification-parameters
source_filename: oneatlas-webhook-notification-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-webhook-notification-parameters-schema.json\",\n  \"title\": \"WebhookNotificationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"description\": \"URL form is verified. To be done: Endpoint need to be validated.\",\n      \"format\": \"url\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-webhook-notification-parameters-schema.json
tags:
- Imagery
- Satellites
title: WebhookNotificationParameters
---
