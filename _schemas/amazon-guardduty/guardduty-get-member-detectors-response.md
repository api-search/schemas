---
description: GetMemberDetectorsResponse schema from Amazon GuardDuty API
layout: schema
name: GetMemberDetectorsResponse
properties_list:
- description: ''
  name: MemberDataSourceConfigurations
  type: object
- description: ''
  name: UnprocessedAccounts
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-member-detectors-response-schema.json
slug: guardduty-get-member-detectors-response
source_filename: guardduty-get-member-detectors-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-member-detectors-response-schema.json\",\n  \"title\": \"GetMemberDetectorsResponse\",\n  \"description\": \"GetMemberDetectorsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MemberDataSourceConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberDataSourceConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"members\"\n          },\n          \"description\": \"An object that describes which data sources are enabled for a member account.\"\n        }\n      ]\n    },\n    \"UnprocessedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedAccounts\"\n        },\n        {\n          \"xml\": {\n            \"name\":\
  \ \"unprocessedAccounts\"\n          },\n          \"description\": \"A list of member account IDs that were unable to be processed along with an explanation for why they were not processed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MemberDataSourceConfigurations\",\n    \"UnprocessedAccounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-member-detectors-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetMemberDetectorsResponse
---
