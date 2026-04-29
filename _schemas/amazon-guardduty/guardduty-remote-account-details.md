---
description: Contains details about the remote Amazon Web Services account that made the API call.
layout: schema
name: RemoteAccountDetails
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Affiliated
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-remote-account-details-schema.json
slug: guardduty-remote-account-details
source_filename: guardduty-remote-account-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-remote-account-details-schema.json\",\n  \"title\": \"RemoteAccountDetails\",\n  \"description\": \"Contains details about the remote Amazon Web Services account that made the API call.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The Amazon Web Services account ID of the remote API caller.\"\n        }\n      ]\n    },\n    \"Affiliated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"affiliated\"\n          },\n          \"description\": \"Details on\
  \ whether the Amazon Web Services account of the remote API caller is related to your GuardDuty environment. If this value is <code>True</code> the API caller is affiliated to your account in some way. If it is <code>False</code> the API caller is from outside your environment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-remote-account-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RemoteAccountDetails
---
