---
description: Contains information about the account.
layout: schema
name: AccountDetail
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Email
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-account-detail-schema.json
slug: guardduty-account-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-account-detail-schema.json\",\n  \"title\": \"AccountDetail\",\n  \"description\": \"Contains information about the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The member account ID.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"email\"\n          },\n          \"description\": \"The email address of the member account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n\
  \    \"Email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-account-detail-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AccountDetail
---
