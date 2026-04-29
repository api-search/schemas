---
description: Request body for batch creating commerce payments
layout: schema
name: BatchCreateRequest
properties_list:
- description: List of payments to create
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-batch-create-request-schema.json
slug: commerce-payments-api-batch-create-request
source_filename: commerce-payments-api-batch-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-create-request-schema.json\",\n  \"title\": \"BatchCreateRequest\",\n  \"description\": \"Request body for batch creating commerce payments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of payments to create\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for creating a new commerce payment\",\n        \"required\": [\n          \"properties\"\n        ],\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties to set on the commerce payment\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\"\
  : \"value\"\n            }\n          },\n          \"associations\": {\n            \"type\": \"array\",\n            \"description\": \"Associations to create with other objects\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationInput\"\n            },\n            \"example\": [\n              {\n                \"to\": {\n                  \"id\": {}\n                },\n                \"types\": [\n                  {}\n                ]\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"associations\": [\n            {\n              \"to\": {\n                \"id\": {}\n              },\n              \"types\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-create-request-schema.json
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
title: BatchCreateRequest
---
