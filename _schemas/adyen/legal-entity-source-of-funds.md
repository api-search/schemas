---
description: SourceOfFunds schema from Adyen API
layout: schema
name: SourceOfFunds
properties_list:
- description: The unique identifier of the business line that will be the source of funds.This must be a business line for a **receivePayments** or **receiveFromPlatformPayments** capability.
  name: acquiringBusinessLineId
  type: string
- description: Indicates whether the funds are coming from transactions processed by Adyen. If **false**, a `description` is required.
  name: adyenProcessedFunds
  type: boolean
- description: Text describing the source of funds. For example, for `type` **business**, provide a description of where the business transactions come from, such as payments through bank transfer. Required when `ad
  name: description
  type: string
- description: 'The type of the source of funds. Possible value: **business**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-source-of-funds-schema.json
slug: legal-entity-source-of-funds
source_filename: legal-entity-source-of-funds-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-source-of-funds-schema.json\",\n  \"title\": \"SourceOfFunds\",\n  \"description\": \"SourceOfFunds schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acquiringBusinessLineId\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"3\",\n      \"x-deprecatedMessage\": \"This field will be removed in v4.\",\n      \"description\": \"The unique identifier of the business line that will be the source of funds.This must be a business line for a **receivePayments** or **receiveFromPlatformPayments** capability.\",\n      \"type\": \"string\"\n    },\n    \"adyenProcessedFunds\": {\n      \"description\": \"Indicates whether the funds are coming from transactions processed by Adyen. If **false**, a `description` is required.\",\n      \"type\": \"boolean\"\n    },\n\
  \    \"description\": {\n      \"description\": \"Text describing the source of funds. For example, for `type` **business**, provide a description of where the business transactions come from, such as payments through bank transfer. Required when `adyenProcessedFunds` is **false**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of the source of funds. Possible value: **business**.\",\n      \"enum\": [\n        \"business\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-source-of-funds-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SourceOfFunds
---
