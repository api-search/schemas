---
description: StopMonitoringMembersRequest schema from Amazon GuardDuty API
layout: schema
name: StopMonitoringMembersRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-stop-monitoring-members-request-schema.json
slug: guardduty-stop-monitoring-members-request
source_filename: guardduty-stop-monitoring-members-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-stop-monitoring-members-request-schema.json\",\n  \"title\": \"StopMonitoringMembersRequest\",\n  \"description\": \"StopMonitoringMembersRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"A list of account IDs for the member accounts to stop monitoring.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-stop-monitoring-members-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: StopMonitoringMembersRequest
---
