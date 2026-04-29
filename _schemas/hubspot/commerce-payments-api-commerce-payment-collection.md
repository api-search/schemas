---
description: A paginated collection of commerce payments
layout: schema
name: CommercePaymentCollection
properties_list:
- description: The list of commerce payments
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-commerce-payment-collection-schema.json
slug: commerce-payments-api-commerce-payment-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-collection-schema.json\",\n  \"title\": \"CommercePaymentCollection\",\n  \"description\": \"A paginated collection of commerce payments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The list of commerce payments\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A commerce payment object representing a payment transaction\",\n        \"required\": [\n          \"id\",\n          \"properties\",\n          \"createdAt\",\n          \"updatedAt\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the commerce payment\",\n            \"example\": \"500123\"\n         \
  \ },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties of the commerce payment\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the commerce payment was created\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the commerce payment was last updated\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the commerce payment is archived\",\n            \"example\": true\n          },\n\
  \          \"archivedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the commerce payment was archived\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"associations\": {\n            \"type\": \"object\",\n            \"description\": \"Associated objects\",\n            \"additionalProperties\": {\n              \"$ref\": \"#/components/schemas/AssociationResult\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"propertiesWithHistory\": {\n            \"type\": \"object\",\n            \"description\": \"Properties with their value history\",\n            \"additionalProperties\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/components/schemas/PropertyHistory\"\n              }\n            },\n            \"example\": {\n              \"key\": \"value\"\n     \
  \       }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true,\n          \"archivedAt\": \"2025-03-15T14:30:00Z\",\n          \"associations\": {\n            \"key\": \"value\"\n          },\n          \"propertiesWithHistory\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Link to the next page\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          }\n        },\n        \"prev\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"before\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the previous page\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the previous page\"\n            }\n          },\n          \"example\": {\n            \"before\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-collection-schema.json
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
title: CommercePaymentCollection
---
