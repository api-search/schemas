---
description: CreateOrderInput schema from Amazon Outposts
layout: schema
name: CreateOrderInput
properties_list:
- description: ''
  name: OutpostIdentifier
  type: object
- description: ''
  name: LineItems
  type: object
- description: ''
  name: PaymentOption
  type: object
- description: ''
  name: PaymentTerm
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-create-order-input-schema.json
slug: openapi-create-order-input
source_filename: openapi-create-order-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-order-input-schema.json\",\n  \"title\": \"CreateOrderInput\",\n  \"description\": \"CreateOrderInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutpostIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutpostIdentifier\"\n        },\n        {\n          \"description\": \" The ID or the Amazon Resource Name (ARN) of the Outpost. \"\n        }\n      ]\n    },\n    \"LineItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemRequestListDefinition\"\n        },\n        {\n          \"description\": \"The line items that make up the order.\"\n        }\n      ]\n    },\n    \"PaymentOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaymentOption\"\
  \n        },\n        {\n          \"description\": \"The payment option.\"\n        }\n      ]\n    },\n    \"PaymentTerm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaymentTerm\"\n        },\n        {\n          \"description\": \"The payment terms.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutpostIdentifier\",\n    \"LineItems\",\n    \"PaymentOption\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-order-input-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: CreateOrderInput
---
