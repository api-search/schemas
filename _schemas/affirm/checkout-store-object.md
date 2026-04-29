---
description: Address details for in-store transactions where the purchase is made at a physical merchant location.
layout: schema
name: StoreObject
properties_list:
- description: Store location name.
  name: name
  type: string
- description: ''
  name: address
  type: object
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-store-object-schema.json
slug: checkout-store-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-store-object-schema.json\",\n  \"title\": \"StoreObject\",\n  \"description\": \"Address details for in-store transactions where the purchase is made at a physical merchant location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Store location name.\",\n      \"example\": \"Example Merchant\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/AddressObject\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-store-object-schema.json
tags: []
title: StoreObject
---
