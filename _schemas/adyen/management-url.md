---
description: Url schema from Adyen API
layout: schema
name: Url
properties_list:
- description: Indicates if the message sent to this URL should be encrypted.
  name: encrypted
  type: boolean
- description: The password for authentication of the notifications.
  name: password
  type: string
- description: 'The URL in the format: http(s)://domain.com.'
  name: url
  type: string
- description: The username for authentication of the notifications.
  name: username
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-url-schema.json
slug: management-url
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-url-schema.json\",\n  \"title\": \"Url\",\n  \"description\": \"Url schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encrypted\": {\n      \"description\": \"Indicates if the message sent to this URL should be encrypted.\",\n      \"type\": \"boolean\"\n    },\n    \"password\": {\n      \"description\": \"The password for authentication of the notifications.\",\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"The URL in the format: http(s)://domain.com.\",\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"description\": \"The username for authentication of the notifications.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-url-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Url
---
