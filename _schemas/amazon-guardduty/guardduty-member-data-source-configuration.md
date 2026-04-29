---
description: Contains information on which data sources are enabled for a member account.
layout: schema
name: MemberDataSourceConfiguration
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
schema_file: json-schema/guardduty-member-data-source-configuration-schema.json
slug: guardduty-member-data-source-configuration
source_filename: guardduty-member-data-source-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-data-source-configuration-schema.json\",\n  \"title\": \"MemberDataSourceConfiguration\",\n  \"description\": \"Contains information on which data sources are enabled for a member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The account ID for the member account.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceConfigurationsResult\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n  \
  \        },\n          \"description\": \"Contains information on the status of data sources for the account.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberFeaturesConfigurationsResults\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"Contains information about the status of the features for the member account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-data-source-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: MemberDataSourceConfiguration
---
