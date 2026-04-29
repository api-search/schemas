---
description: ListLongTermPricingResult schema from Amazon Snow Family API
layout: schema
name: ListLongTermPricingResult
properties_list:
- description: ''
  name: LongTermPricingEntries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-long-term-pricing-result-schema.json
slug: amazon-snow-family-list-long-term-pricing-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-long-term-pricing-result-schema.json\",\n  \"title\": \"ListLongTermPricingResult\",\n  \"description\": \"ListLongTermPricingResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LongTermPricingEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingEntryList\"\n        },\n        {\n          \"description\": \"Each <code>LongTermPricingEntry</code> object contains a status, ID, and other information about the <code>LongTermPricing</code> type. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Because HTTP requests are stateless, this is the starting\
  \ point for your next list of returned <code>ListLongTermPricing</code> list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-long-term-pricing-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListLongTermPricingResult
---
