---
description: KlarnaInfo schema from Adyen API
layout: schema
name: KlarnaInfo
properties_list:
- description: 'Indicates the status of [Automatic capture](https://docs.adyen.com/online-payments/capture#automatic-capture). Default value: **false**.'
  name: autoCapture
  type: boolean
- description: The email address for disputes.
  name: disputeEmail
  type: string
- description: The region of operation. For example, **NA**, **EU**, **CH**, **AU**.
  name: region
  type: string
- description: The email address of merchant support.
  name: supportEmail
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-klarna-info-schema.json
slug: management-klarna-info
source_filename: management-klarna-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-klarna-info-schema.json\",\n  \"title\": \"KlarnaInfo\",\n  \"description\": \"KlarnaInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoCapture\": {\n      \"description\": \"Indicates the status of [Automatic capture](https://docs.adyen.com/online-payments/capture#automatic-capture). Default value: **false**.\",\n      \"type\": \"boolean\"\n    },\n    \"disputeEmail\": {\n      \"description\": \"The email address for disputes.\",\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"description\": \"The region of operation. For example, **NA**, **EU**, **CH**, **AU**.\",\n      \"enum\": [\n        \"NA\",\n        \"EU\",\n        \"CH\",\n        \"AU\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n\
  \    \"supportEmail\": {\n      \"description\": \"The email address of merchant support.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"region\",\n    \"supportEmail\",\n    \"disputeEmail\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-klarna-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KlarnaInfo
---
