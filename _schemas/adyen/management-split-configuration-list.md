---
description: SplitConfigurationList schema from Adyen API
layout: schema
name: SplitConfigurationList
properties_list:
- description: List of split configurations applied to the stores under the merchant account.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-split-configuration-list-schema.json
slug: management-split-configuration-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-split-configuration-list-schema.json\",\n  \"title\": \"SplitConfigurationList\",\n  \"description\": \"SplitConfigurationList schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"List of split configurations applied to the stores under the merchant account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SplitConfiguration\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-split-configuration-list-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SplitConfigurationList
---
