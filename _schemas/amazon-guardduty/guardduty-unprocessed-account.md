---
description: Contains information about the accounts that weren't processed.
layout: schema
name: UnprocessedAccount
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Result
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-unprocessed-account-schema.json
slug: guardduty-unprocessed-account
source_filename: guardduty-unprocessed-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-unprocessed-account-schema.json\",\n  \"title\": \"UnprocessedAccount\",\n  \"description\": \"Contains information about the accounts that weren't processed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"Result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"result\"\n          },\n          \"description\": \"A reason why the account hasn't been processed.\"\n        }\n    \
  \  ]\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n    \"Result\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-unprocessed-account-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UnprocessedAccount
---
