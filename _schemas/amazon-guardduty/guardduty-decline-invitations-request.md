---
description: DeclineInvitationsRequest schema from Amazon GuardDuty API
layout: schema
name: DeclineInvitationsRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-decline-invitations-request-schema.json
slug: guardduty-decline-invitations-request
source_filename: guardduty-decline-invitations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-decline-invitations-request-schema.json\",\n  \"title\": \"DeclineInvitationsRequest\",\n  \"description\": \"DeclineInvitationsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"A list of account IDs of the Amazon Web Services accounts that sent invitations to the current member account that you want to decline invitations from.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-decline-invitations-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DeclineInvitationsRequest
---
