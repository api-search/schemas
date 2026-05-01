---
description: GetRemainingFreeTrialDaysResponse schema from Amazon GuardDuty API
layout: schema
name: GetRemainingFreeTrialDaysResponse
properties_list:
- description: ''
  name: Accounts
  type: object
- description: ''
  name: UnprocessedAccounts
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-remaining-free-trial-days-response-schema.json
slug: guardduty-get-remaining-free-trial-days-response
source_filename: guardduty-get-remaining-free-trial-days-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-remaining-free-trial-days-response-schema.json\",\n  \"title\": \"GetRemainingFreeTrialDaysResponse\",\n  \"description\": \"GetRemainingFreeTrialDaysResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountFreeTrialInfos\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accounts\"\n          },\n          \"description\": \"The member accounts which were included in a request and were processed successfully.\"\n        }\n      ]\n    },\n    \"UnprocessedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedAccounts\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"unprocessedAccounts\"\n          },\n          \"description\": \"The member account that was included in a request but for which the request could not be processed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-remaining-free-trial-days-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetRemainingFreeTrialDaysResponse
---
