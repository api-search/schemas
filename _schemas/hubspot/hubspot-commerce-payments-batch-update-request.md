---
description: Request body for batch updating commerce payments
layout: schema
name: BatchUpdateRequest
properties_list:
- description: List of payments to update
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-batch-update-request-schema.json
slug: hubspot-commerce-payments-batch-update-request
source_filename: hubspot-commerce-payments-batch-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch updating commerce payments\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of payments to update\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"idProperty\": \"500123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single input item for batch update\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the payment to update\",\n            \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties to update\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"idProperty\": {\n\
  \            \"type\": \"string\",\n            \"description\": \"The property to use as the identifier\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"properties\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-batch-update-request-schema.json
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
title: BatchUpdateRequest
---
