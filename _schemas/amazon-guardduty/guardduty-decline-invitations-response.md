---
description: DeclineInvitationsResponse schema from Amazon GuardDuty API
layout: schema
name: DeclineInvitationsResponse
properties_list:
- description: ''
  name: UnprocessedAccounts
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-decline-invitations-response-schema.json
slug: guardduty-decline-invitations-response
source_filename: guardduty-decline-invitations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-decline-invitations-response-schema.json\",\n  \"title\": \"DeclineInvitationsResponse\",\n  \"description\": \"DeclineInvitationsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedAccounts\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unprocessedAccounts\"\n          },\n          \"description\": \"A list of objects that contain the unprocessed account and a result string that explains why it was unprocessed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UnprocessedAccounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-decline-invitations-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DeclineInvitationsResponse
---
