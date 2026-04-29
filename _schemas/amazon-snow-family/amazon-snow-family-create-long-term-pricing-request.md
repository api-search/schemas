---
description: CreateLongTermPricingRequest schema from Amazon Snow Family API
layout: schema
name: CreateLongTermPricingRequest
properties_list:
- description: ''
  name: LongTermPricingType
  type: object
- description: ''
  name: IsLongTermPricingAutoRenew
  type: object
- description: ''
  name: SnowballType
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-long-term-pricing-request-schema.json
slug: amazon-snow-family-create-long-term-pricing-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-long-term-pricing-request-schema.json\",\n  \"title\": \"CreateLongTermPricingRequest\",\n  \"description\": \"CreateLongTermPricingRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LongTermPricingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingType\"\n        },\n        {\n          \"description\": \"The type of long-term pricing option you want for the device, either 1-year or 3-year long-term pricing.\"\n        }\n      ]\n    },\n    \"IsLongTermPricingAutoRenew\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JavaBoolean\"\n        },\n        {\n          \"description\": \"Specifies whether the current long-term pricing type for the device\
  \ should be renewed.\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\": \"The type of Snow Family devices to use for the long-term pricing job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LongTermPricingType\",\n    \"SnowballType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-long-term-pricing-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateLongTermPricingRequest
---
