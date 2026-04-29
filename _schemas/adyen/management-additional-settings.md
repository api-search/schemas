---
description: AdditionalSettings schema from Adyen API
layout: schema
name: AdditionalSettings
properties_list:
- description: Object containing list of event codes for which the notifcation will be sent.
  name: includeEventCodes
  type: array
- description: 'Object containing boolean key-value pairs. The key can be any [standard webhook additional setting](https://docs.adyen.com/development-resources/webhooks/additional-settings), and the value indicates '
  name: properties
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-additional-settings-schema.json
slug: management-additional-settings
source_filename: management-additional-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-additional-settings-schema.json\",\n  \"title\": \"AdditionalSettings\",\n  \"description\": \"AdditionalSettings schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"includeEventCodes\": {\n      \"description\": \"Object containing list of event codes for which the notifcation will be sent. \",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"properties\": {\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      },\n      \"description\": \"Object containing boolean key-value pairs. The key can be any [standard webhook additional setting](https://docs.adyen.com/development-resources/webhooks/additional-settings), and the value indicates if the setting is enabled.\\nFor example, `captureDelayHours`: **true**\
  \ means the standard notifications you get will contain the number of hours remaining until the payment will be captured.\",\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-additional-settings-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalSettings
---
