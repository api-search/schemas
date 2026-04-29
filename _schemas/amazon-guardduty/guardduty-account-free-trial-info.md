---
description: Provides details of the GuardDuty member account that uses a free trial service.
layout: schema
name: AccountFreeTrialInfo
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Features
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-account-free-trial-info-schema.json
slug: guardduty-account-free-trial-info
source_filename: guardduty-account-free-trial-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-account-free-trial-info-schema.json\",\n  \"title\": \"AccountFreeTrialInfo\",\n  \"description\": \"Provides details of the GuardDuty member account that uses a free trial service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The account identifier of the GuardDuty member account.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourcesFreeTrial\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n\
  \          \"description\": \"Describes the data source enabled for the GuardDuty member account.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeTrialFeatureConfigurationsResults\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"A list of features enabled for the GuardDuty account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-account-free-trial-info-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AccountFreeTrialInfo
---
