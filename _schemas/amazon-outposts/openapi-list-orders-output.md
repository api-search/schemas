---
description: ListOrdersOutput schema from Amazon Outposts
layout: schema
name: ListOrdersOutput
properties_list:
- description: ''
  name: Orders
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-list-orders-output-schema.json
slug: openapi-list-orders-output
source_filename: openapi-list-orders-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-orders-output-schema.json\",\n  \"title\": \"ListOrdersOutput\",\n  \"description\": \"ListOrdersOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Orders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderSummaryListDefinition\"\n        },\n        {\n          \"description\": \" Information about the orders. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/Token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-orders-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ListOrdersOutput
---
