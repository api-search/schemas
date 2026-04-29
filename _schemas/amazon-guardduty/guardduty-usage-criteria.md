---
description: Contains information about the criteria used to query usage statistics.
layout: schema
name: UsageCriteria
properties_list:
- description: ''
  name: AccountIds
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Resources
  type: object
- description: ''
  name: Features
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-usage-criteria-schema.json
slug: guardduty-usage-criteria
source_filename: guardduty-usage-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-criteria-schema.json\",\n  \"title\": \"UsageCriteria\",\n  \"description\": \"Contains information about the criteria used to query usage statistics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"The account IDs to aggregate usage statistics from.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceList\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n          \"description\": \"\
  The data sources to aggregate usage statistics from.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resources\"\n          },\n          \"description\": \"The resources to aggregate usage statistics from. Only accepts exact resource names.\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageFeatureList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"The features to aggregate usage statistics from.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-criteria-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UsageCriteria
---
