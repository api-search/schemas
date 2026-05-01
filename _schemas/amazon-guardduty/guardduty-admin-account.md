---
description: The account within the organization specified as the GuardDuty delegated administrator.
layout: schema
name: AdminAccount
properties_list:
- description: ''
  name: AdminAccountId
  type: object
- description: ''
  name: AdminStatus
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-admin-account-schema.json
slug: guardduty-admin-account
source_filename: guardduty-admin-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-admin-account-schema.json\",\n  \"title\": \"AdminAccount\",\n  \"description\": \"The account within the organization specified as the GuardDuty delegated administrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdminAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adminAccountId\"\n          },\n          \"description\": \"The Amazon Web Services account ID for the account.\"\n        }\n      ]\n    },\n    \"AdminStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adminStatus\"\n          },\n          \"description\": \"Indicates whether\
  \ the account is enabled as the delegated administrator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-admin-account-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AdminAccount
---
