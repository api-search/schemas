---
description: ExternalPlatform schema from Adyen API
layout: schema
name: ExternalPlatform
properties_list:
- description: External platform integrator.
  name: integrator
  type: string
- description: Name of the field. For example, Name of External Platform.
  name: name
  type: string
- description: Version of the field. For example, Version of External Platform.
  name: version
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-external-platform-schema.json
slug: payments-external-platform
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-external-platform-schema.json\",\n  \"title\": \"ExternalPlatform\",\n  \"description\": \"ExternalPlatform schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"integrator\": {\n      \"description\": \"External platform integrator.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the field. For example, Name of External Platform.\",\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"Version of the field. For example, Version of External Platform.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-external-platform-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ExternalPlatform
---
