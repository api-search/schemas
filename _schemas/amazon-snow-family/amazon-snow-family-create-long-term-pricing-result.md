---
description: CreateLongTermPricingResult schema from Amazon Snow Family API
layout: schema
name: CreateLongTermPricingResult
properties_list:
- description: ''
  name: LongTermPricingId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-long-term-pricing-result-schema.json
slug: amazon-snow-family-create-long-term-pricing-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-long-term-pricing-result-schema.json\",\n  \"title\": \"CreateLongTermPricingResult\",\n  \"description\": \"CreateLongTermPricingResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LongTermPricingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingId\"\n        },\n        {\n          \"description\": \"The ID of the long-term pricing type for the device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-long-term-pricing-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateLongTermPricingResult
---
