---
description: CreateAddressRequest schema from Amazon Snow Family API
layout: schema
name: CreateAddressRequest
properties_list:
- description: ''
  name: Address
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-address-request-schema.json
slug: amazon-snow-family-create-address-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-address-request-schema.json\",\n  \"title\": \"CreateAddressRequest\",\n  \"description\": \"CreateAddressRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Address\"\n        },\n        {\n          \"description\": \"The address that you want the Snow device shipped to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Address\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-address-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateAddressRequest
---
