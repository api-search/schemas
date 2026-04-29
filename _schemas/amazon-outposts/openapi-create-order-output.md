---
description: CreateOrderOutput schema from Amazon Outposts
layout: schema
name: CreateOrderOutput
properties_list:
- description: ''
  name: Order
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-create-order-output-schema.json
slug: openapi-create-order-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-order-output-schema.json\",\n  \"title\": \"CreateOrderOutput\",\n  \"description\": \"CreateOrderOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Order\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Order\"\n        },\n        {\n          \"description\": \"Information about this order.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-order-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: CreateOrderOutput
---
