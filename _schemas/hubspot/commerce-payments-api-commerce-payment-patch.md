---
description: Input for updating a commerce payment
layout: schema
name: CommercePaymentPatch
properties_list:
- description: The properties to update on the commerce payment
  name: properties
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-commerce-payment-patch-schema.json
slug: commerce-payments-api-commerce-payment-patch
source_filename: commerce-payments-api-commerce-payment-patch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-patch-schema.json\",\n  \"title\": \"CommercePaymentPatch\",\n  \"description\": \"Input for updating a commerce payment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties to update on the commerce payment\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-patch-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: CommercePaymentPatch
---
