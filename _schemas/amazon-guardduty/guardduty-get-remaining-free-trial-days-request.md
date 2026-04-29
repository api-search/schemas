---
description: GetRemainingFreeTrialDaysRequest schema from Amazon GuardDuty API
layout: schema
name: GetRemainingFreeTrialDaysRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-remaining-free-trial-days-request-schema.json
slug: guardduty-get-remaining-free-trial-days-request
source_filename: guardduty-get-remaining-free-trial-days-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-remaining-free-trial-days-request-schema.json\",\n  \"title\": \"GetRemainingFreeTrialDaysRequest\",\n  \"description\": \"GetRemainingFreeTrialDaysRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"A list of account identifiers of the GuardDuty member account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-remaining-free-trial-days-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetRemainingFreeTrialDaysRequest
---
