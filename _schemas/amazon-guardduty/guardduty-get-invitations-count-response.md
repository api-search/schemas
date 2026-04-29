---
description: GetInvitationsCountResponse schema from Amazon GuardDuty API
layout: schema
name: GetInvitationsCountResponse
properties_list:
- description: ''
  name: InvitationsCount
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-invitations-count-response-schema.json
slug: guardduty-get-invitations-count-response
source_filename: guardduty-get-invitations-count-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-invitations-count-response-schema.json\",\n  \"title\": \"GetInvitationsCountResponse\",\n  \"description\": \"GetInvitationsCountResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvitationsCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitationsCount\"\n          },\n          \"description\": \"The number of received invitations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-invitations-count-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetInvitationsCountResponse
---
