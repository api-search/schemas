---
description: BillingEntity schema from Adyen API
layout: schema
name: BillingEntity
properties_list:
- description: The address details of the billing entity.
  name: address
  type: object
- description: The email address of the billing entity.
  name: email
  type: string
- description: The unique identifier of the billing entity, for use as `billingEntityId` when creating an order.
  name: id
  type: string
- description: The unique name of the billing entity.
  name: name
  type: string
- description: The tax number of the billing entity.
  name: taxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-billing-entity-schema.json
slug: management-billing-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-billing-entity-schema.json\",\n  \"title\": \"BillingEntity\",\n  \"description\": \"BillingEntity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address details of the billing entity.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the billing entity.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the billing entity, for use as `billingEntityId` when creating an order.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The unique name of the billing entity.\",\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"description\": \"The tax number of the billing\
  \ entity.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-billing-entity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BillingEntity
---
