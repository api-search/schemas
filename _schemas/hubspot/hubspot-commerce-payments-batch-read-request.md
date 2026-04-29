---
description: Request body for batch reading commerce payments
layout: schema
name: BatchReadRequest
properties_list:
- description: List of payment identifiers to read
  name: inputs
  type: array
- description: Properties to return for each payment
  name: properties
  type: array
- description: Properties to return with history
  name: propertiesWithHistory
  type: array
- description: The property to use as the identifier
  name: idProperty
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-batch-read-request-schema.json
slug: hubspot-commerce-payments-batch-read-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch reading commerce payments\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of payment identifiers to read\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single input item for batch read\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the payment to read\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to return for each payment\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"propertiesWithHistory\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Properties to return with history\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"idProperty\": {\n      \"type\": \"string\",\n      \"description\": \"The property to use as the identifier\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"properties\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchReadRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-batch-read-request-schema.json
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
title: BatchReadRequest
---
