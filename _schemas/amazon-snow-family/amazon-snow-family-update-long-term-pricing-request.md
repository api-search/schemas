---
description: UpdateLongTermPricingRequest schema from Amazon Snow Family API
layout: schema
name: UpdateLongTermPricingRequest
properties_list:
- description: ''
  name: LongTermPricingId
  type: object
- description: ''
  name: ReplacementJob
  type: object
- description: ''
  name: IsLongTermPricingAutoRenew
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-update-long-term-pricing-request-schema.json
slug: amazon-snow-family-update-long-term-pricing-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-long-term-pricing-request-schema.json\",\n  \"title\": \"UpdateLongTermPricingRequest\",\n  \"description\": \"UpdateLongTermPricingRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LongTermPricingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingId\"\n        },\n        {\n          \"description\": \"The ID of the long-term pricing type for the device.\"\n        }\n      ]\n    },\n    \"ReplacementJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"Specifies that a device that is ordered with long-term pricing should be replaced with a new device.\"\n        }\n      ]\n    },\n   \
  \ \"IsLongTermPricingAutoRenew\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JavaBoolean\"\n        },\n        {\n          \"description\": \"If set to <code>true</code>, specifies that the current long-term pricing type for the device should be automatically renewed before the long-term pricing contract expires.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LongTermPricingId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-long-term-pricing-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: UpdateLongTermPricingRequest
---
