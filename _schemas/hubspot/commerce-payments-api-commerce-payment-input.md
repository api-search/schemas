---
description: Input for creating a new commerce payment
layout: schema
name: CommercePaymentInput
properties_list:
- description: The properties to set on the commerce payment
  name: properties
  type: object
- description: Associations to create with other objects
  name: associations
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-commerce-payment-input-schema.json
slug: commerce-payments-api-commerce-payment-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-input-schema.json\",\n  \"title\": \"CommercePaymentInput\",\n  \"description\": \"Input for creating a new commerce payment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties to set on the commerce payment\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"Associations to create with other objects\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for creating an association\",\n        \"required\": [\n          \"to\",\n          \"types\"\n        ],\n        \"properties\"\
  : {\n          \"to\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"id\"\n            ],\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the object to associate with\"\n              }\n            },\n            \"example\": {\n              \"id\": \"500123\"\n            }\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"description\": \"The association types\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationType\"\n            },\n            \"example\": [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n                \"associationTypeId\": 500123\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"to\": {\n            \"id\": {}\n          },\n          \"types\": [\n            {}\n\
  \          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-commerce-payment-input-schema.json
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
title: CommercePaymentInput
---
