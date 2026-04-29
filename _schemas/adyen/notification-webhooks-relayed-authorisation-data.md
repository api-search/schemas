---
description: RelayedAuthorisationData schema from Adyen API
layout: schema
name: RelayedAuthorisationData
properties_list:
- description: The `metadata` object from the relayed authorisation response from your server.
  name: metadata
  type: object
- description: The `reference` from the relayed authorisation response from your server.
  name: reference
  type: string
- description: The value can be **Authorised** or **Refused**, based on the `authorisationDecision.status` in the relayed authorisation response from your server.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-relayed-authorisation-data-schema.json
slug: notification-webhooks-relayed-authorisation-data
source_filename: notification-webhooks-relayed-authorisation-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-relayed-authorisation-data-schema.json\",\n  \"title\": \"RelayedAuthorisationData\",\n  \"description\": \"RelayedAuthorisationData schema from Adyen API\",\n  \"properties\": {\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The `metadata` object from the relayed authorisation response from your server.\",\n      \"type\": \"object\"\n    },\n    \"reference\": {\n      \"description\": \"The `reference` from the relayed authorisation response from your server.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The value can be **Authorised** or **Refused**, based on the `authorisationDecision.status` in the relayed authorisation response from your server.\",\n      \"type\": \"string\"\
  \n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-relayed-authorisation-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RelayedAuthorisationData
---
