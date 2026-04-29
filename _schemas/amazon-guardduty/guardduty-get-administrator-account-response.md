---
description: GetAdministratorAccountResponse schema from Amazon GuardDuty API
layout: schema
name: GetAdministratorAccountResponse
properties_list:
- description: ''
  name: Administrator
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-administrator-account-response-schema.json
slug: guardduty-get-administrator-account-response
source_filename: guardduty-get-administrator-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-administrator-account-response-schema.json\",\n  \"title\": \"GetAdministratorAccountResponse\",\n  \"description\": \"GetAdministratorAccountResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Administrator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Administrator\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"administrator\"\n          },\n          \"description\": \"The administrator account details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Administrator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-administrator-account-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetAdministratorAccountResponse
---
