---
description: A commerce payment object representing a payment transaction
layout: schema
name: CommercePayment
properties_list:
- description: The unique identifier of the commerce payment
  name: id
  type: string
- description: The properties of the commerce payment
  name: properties
  type: object
- description: When the commerce payment was created
  name: createdAt
  type: string
- description: When the commerce payment was last updated
  name: updatedAt
  type: string
- description: Whether the commerce payment is archived
  name: archived
  type: boolean
- description: When the commerce payment was archived
  name: archivedAt
  type: string
- description: Associated objects
  name: associations
  type: object
- description: Properties with their value history
  name: propertiesWithHistory
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-commerce-payment-schema.json
slug: commerce-payments-api-commerce-payment
source_filename: commerce-payments-api-commerce-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-schema.json\",\n  \"title\": \"CommercePayment\",\n  \"description\": \"A commerce payment object representing a payment transaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the commerce payment\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties of the commerce payment\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the commerce payment was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\
  \n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the commerce payment was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the commerce payment is archived\",\n      \"example\": true\n    },\n    \"archivedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the commerce payment was archived\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"description\": \"Associated objects\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"description\": \"Association results for an object\",\n        \"properties\": {\n          \"results\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n  \
  \              \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"example\": [\n              {\n                \"id\": \"500123\",\n                \"type\": \"standard\"\n              }\n            ]\n          },\n          \"paging\": {\n            \"$ref\": \"#/components/schemas/Paging\"\n          }\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"propertiesWithHistory\": {\n      \"type\": \"object\",\n      \"description\": \"Properties with their value history\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"description\": \"A historical property value\",\n          \"required\": [\n            \"value\",\n            \"timestamp\",\n            \"sourceType\"\n          ],\n          \"properties\"\
  : {\n            \"value\": {\n              \"type\": \"string\",\n              \"description\": \"The property value\",\n              \"example\": \"example-value\"\n            },\n            \"timestamp\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"When this value was set\",\n              \"example\": \"2025-03-15T14:30:00Z\"\n            },\n            \"sourceType\": {\n              \"type\": \"string\",\n              \"description\": \"The source that set this value\",\n              \"example\": \"standard\"\n            },\n            \"sourceId\": {\n              \"type\": \"string\",\n              \"description\": \"The identifier of the source\",\n              \"example\": \"500123\"\n            },\n            \"sourceLabel\": {\n              \"type\": \"string\",\n              \"description\": \"A human-readable label for the source\",\n              \"example\": \"Example Record\"\n   \
  \         },\n            \"updatedByUserId\": {\n              \"type\": \"integer\",\n              \"description\": \"The user ID that made the change\",\n              \"example\": 1718153645993\n            }\n          }\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"properties\",\n    \"createdAt\",\n    \"updatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-schema.json
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
title: CommercePayment
---
