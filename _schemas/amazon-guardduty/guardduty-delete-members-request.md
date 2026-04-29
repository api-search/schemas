---
description: DeleteMembersRequest schema from Amazon GuardDuty API
layout: schema
name: DeleteMembersRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-delete-members-request-schema.json
slug: guardduty-delete-members-request
source_filename: guardduty-delete-members-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-delete-members-request-schema.json\",\n  \"title\": \"DeleteMembersRequest\",\n  \"description\": \"DeleteMembersRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"A list of account IDs of the GuardDuty member accounts that you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-delete-members-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DeleteMembersRequest
---
