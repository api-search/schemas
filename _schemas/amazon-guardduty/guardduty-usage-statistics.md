---
description: Contains the result of GuardDuty usage. If a UsageStatisticType is provided the result for other types will be null.
layout: schema
name: UsageStatistics
properties_list:
- description: ''
  name: SumByAccount
  type: object
- description: ''
  name: SumByDataSource
  type: object
- description: ''
  name: SumByResource
  type: object
- description: ''
  name: TopResources
  type: object
- description: ''
  name: SumByFeature
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-usage-statistics-schema.json
slug: guardduty-usage-statistics
source_filename: guardduty-usage-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-statistics-schema.json\",\n  \"title\": \"UsageStatistics\",\n  \"description\": \"Contains the result of GuardDuty usage. If a UsageStatisticType is provided the result for other types will be null. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SumByAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageAccountResultList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sumByAccount\"\n          },\n          \"description\": \"The usage statistic sum organized by account ID.\"\n        }\n      ]\n    },\n    \"SumByDataSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageDataSourceResultList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sumByDataSource\"\
  \n          },\n          \"description\": \"The usage statistic sum organized by on data source.\"\n        }\n      ]\n    },\n    \"SumByResource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageResourceResultList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sumByResource\"\n          },\n          \"description\": \"The usage statistic sum organized by resource.\"\n        }\n      ]\n    },\n    \"TopResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageResourceResultList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"topResources\"\n          },\n          \"description\": \"Lists the top 50 resources that have generated the most GuardDuty usage, in order from most to least expensive.\"\n        }\n      ]\n    },\n    \"SumByFeature\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageFeatureResultList\"\n        },\n  \
  \      {\n          \"xml\": {\n            \"name\": \"sumByFeature\"\n          },\n          \"description\": \"The usage statistic sum organized by feature.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-statistics-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UsageStatistics
---
