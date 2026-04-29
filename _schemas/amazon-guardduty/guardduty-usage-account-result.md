---
description: Contains information on the total of usage based on account IDs.
layout: schema
name: UsageAccountResult
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Total
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-usage-account-result-schema.json
slug: guardduty-usage-account-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-account-result-schema.json\",\n  \"title\": \"UsageAccountResult\",\n  \"description\": \"Contains information on the total of usage based on account IDs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The Account ID that generated usage.\"\n        }\n      ]\n    },\n    \"Total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Total\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"total\"\n          },\n          \"description\": \"Represents the total of usage for the Account ID.\"\n        }\n  \
  \    ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-account-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UsageAccountResult
---
