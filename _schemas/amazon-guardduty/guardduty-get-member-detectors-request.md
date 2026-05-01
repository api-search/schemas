---
description: GetMemberDetectorsRequest schema from Amazon GuardDuty API
layout: schema
name: GetMemberDetectorsRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-member-detectors-request-schema.json
slug: guardduty-get-member-detectors-request
source_filename: guardduty-get-member-detectors-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-member-detectors-request-schema.json\",\n  \"title\": \"GetMemberDetectorsRequest\",\n  \"description\": \"GetMemberDetectorsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"The account ID of the member account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-member-detectors-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetMemberDetectorsRequest
---
