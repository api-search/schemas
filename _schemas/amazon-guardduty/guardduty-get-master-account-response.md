---
description: This output is deprecated, use GetAdministratorAccountResponse instead
layout: schema
name: GetMasterAccountResponse
properties_list:
- description: ''
  name: Master
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-master-account-response-schema.json
slug: guardduty-get-master-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-master-account-response-schema.json\",\n  \"title\": \"GetMasterAccountResponse\",\n  \"description\": \"This output is deprecated, use GetAdministratorAccountResponse instead\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Master\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Master\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"master\"\n          },\n          \"description\": \"The administrator account details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Master\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-master-account-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetMasterAccountResponse
---
