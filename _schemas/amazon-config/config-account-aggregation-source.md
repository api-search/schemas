---
description: A collection of accounts and regions.
layout: schema
name: AccountAggregationSource
properties_list:
- description: ''
  name: AccountIds
  type: object
- description: ''
  name: AllAwsRegions
  type: object
- description: ''
  name: AwsRegions
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-account-aggregation-source-schema.json
slug: config-account-aggregation-source
source_filename: config-account-aggregation-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-account-aggregation-source-schema.json\",\n  \"title\": \"AccountAggregationSource\",\n  \"description\": \"A collection of accounts and regions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAggregationSourceAccountList\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the account being aggregated. \"\n        }\n      ]\n    },\n    \"AllAwsRegions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"If true, aggregate existing Config regions and future regions.\"\n        }\n      ]\n    },\n    \"AwsRegions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatorRegionList\"\
  \n        },\n        {\n          \"description\": \"The source regions being aggregated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-account-aggregation-source-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: AccountAggregationSource
---
