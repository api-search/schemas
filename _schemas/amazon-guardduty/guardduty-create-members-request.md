---
description: CreateMembersRequest schema from Amazon GuardDuty API
layout: schema
name: CreateMembersRequest
properties_list:
- description: ''
  name: AccountDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-members-request-schema.json
slug: guardduty-create-members-request
source_filename: guardduty-create-members-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-members-request-schema.json\",\n  \"title\": \"CreateMembersRequest\",\n  \"description\": \"CreateMembersRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountDetails\"\n          },\n          \"description\": \"A list of account ID and email address pairs of the accounts that you want to associate with the GuardDuty administrator account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-members-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreateMembersRequest
---
