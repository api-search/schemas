---
description: CreateMembersResponse schema from Amazon GuardDuty API
layout: schema
name: CreateMembersResponse
properties_list:
- description: ''
  name: UnprocessedAccounts
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-members-response-schema.json
slug: guardduty-create-members-response
source_filename: guardduty-create-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-members-response-schema.json\",\n  \"title\": \"CreateMembersResponse\",\n  \"description\": \"CreateMembersResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedAccounts\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unprocessedAccounts\"\n          },\n          \"description\": \"A list of objects that include the <code>accountIds</code> of the unprocessed accounts and a result string that explains why each was unprocessed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UnprocessedAccounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-members-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreateMembersResponse
---
