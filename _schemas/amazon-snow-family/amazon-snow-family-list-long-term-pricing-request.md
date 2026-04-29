---
description: ListLongTermPricingRequest schema from Amazon Snow Family API
layout: schema
name: ListLongTermPricingRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-long-term-pricing-request-schema.json
slug: amazon-snow-family-list-long-term-pricing-request
source_filename: amazon-snow-family-list-long-term-pricing-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-long-term-pricing-request-schema.json\",\n  \"title\": \"ListLongTermPricingRequest\",\n  \"description\": \"ListLongTermPricingRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListLimit\"\n        },\n        {\n          \"description\": \"The maximum number of <code>ListLongTermPricing</code> objects to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Because HTTP requests are stateless, this is the starting point for your next list of <code>ListLongTermPricing</code> to return.\"\n      \
  \  }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-long-term-pricing-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListLongTermPricingRequest
---
