---
description: RemediatingAction schema from Adyen API
layout: schema
name: RemediatingAction
properties_list:
- description: The remediating action code.
  name: code
  type: string
- description: A description of how you can resolve the verification error.
  name: message
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-remediating-action-schema.json
slug: notification-webhooks-remediating-action
source_filename: notification-webhooks-remediating-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-remediating-action-schema.json\",\n  \"title\": \"RemediatingAction\",\n  \"description\": \"RemediatingAction schema from Adyen API\",\n  \"properties\": {\n    \"code\": {\n      \"description\": \"The remediating action code.\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"A description of how you can resolve the verification error.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-remediating-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RemediatingAction
---
