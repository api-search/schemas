---
description: SDKEphemPubKey schema from Adyen API
layout: schema
name: SDKEphemPubKey
properties_list:
- description: The `crv` value as received from the 3D Secure 2 SDK.
  name: crv
  type: string
- description: The `kty` value as received from the 3D Secure 2 SDK.
  name: kty
  type: string
- description: The `x` value as received from the 3D Secure 2 SDK.
  name: x
  type: string
- description: The `y` value as received from the 3D Secure 2 SDK.
  name: y
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-sdk-ephem-pub-key-schema.json
slug: payments-sdk-ephem-pub-key
source_filename: payments-sdk-ephem-pub-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-sdk-ephem-pub-key-schema.json\",\n  \"title\": \"SDKEphemPubKey\",\n  \"description\": \"SDKEphemPubKey schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crv\": {\n      \"description\": \"The `crv` value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    },\n    \"kty\": {\n      \"description\": \"The `kty` value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    },\n    \"x\": {\n      \"description\": \"The `x` value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    },\n    \"y\": {\n      \"description\": \"The `y` value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-sdk-ephem-pub-key-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SDKEphemPubKey
---
