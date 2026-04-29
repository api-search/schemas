---
description: A single input item for batch update
layout: schema
name: BatchUpdateInputItem
properties_list:
- description: The ID of the payment to update
  name: id
  type: string
- description: The properties to update
  name: properties
  type: object
- description: The property to use as the identifier
  name: idProperty
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-batch-update-input-item-schema.json
slug: commerce-payments-api-batch-update-input-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-update-input-item-schema.json\",\n  \"title\": \"BatchUpdateInputItem\",\n  \"description\": \"A single input item for batch update\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the payment to update\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties to update\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"idProperty\": {\n      \"type\": \"string\",\n      \"description\": \"The property to use as the identifier\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"properties\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-update-input-item-schema.json
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
title: BatchUpdateInputItem
---
