---
description: This input is deprecated, use AcceptAdministratorInvitationRequest instead
layout: schema
name: AcceptInvitationRequest
properties_list:
- description: ''
  name: MasterId
  type: object
- description: ''
  name: InvitationId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-accept-invitation-request-schema.json
slug: guardduty-accept-invitation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-accept-invitation-request-schema.json\",\n  \"title\": \"AcceptInvitationRequest\",\n  \"description\": \"This input is deprecated, use AcceptAdministratorInvitationRequest instead\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MasterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"masterId\"\n          },\n          \"description\": \"The account ID of the GuardDuty administrator account whose invitation you're accepting.\"\n        }\n      ]\n    },\n    \"InvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitationId\"\n          },\n          \"description\"\
  : \"The value that is used to validate the administrator account to the member account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MasterId\",\n    \"InvitationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-accept-invitation-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AcceptInvitationRequest
---
