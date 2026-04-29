---
description: It contains information related to the security of the message. SecurityTrailer as used by Adyen.
layout: schema
name: SecurityTrailer
properties_list:
- description: ''
  name: AdyenCryptoVersion
  type: integer
- description: ''
  name: KeyIdentifier
  type: string
- description: ''
  name: KeyVersion
  type: integer
- description: ''
  name: Nonce
  type: string
- description: ''
  name: Hmac
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-security-trailer-schema.json
slug: terminal-security-trailer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-security-trailer-schema.json\",\n  \"title\": \"SecurityTrailer\",\n  \"description\": \"It contains information related to the security of the message. SecurityTrailer as used by Adyen.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdyenCryptoVersion\": {\n      \"type\": \"integer\"\n    },\n    \"KeyIdentifier\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"KeyVersion\": {\n      \"type\": \"integer\"\n    },\n    \"Nonce\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\"\n    },\n    \"Hmac\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"AdyenCryptoVersion\",\n    \"KeyIdentifier\",\n    \"KeyVersion\",\n    \"Nonce\",\n    \"Hmac\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-security-trailer-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SecurityTrailer
---
