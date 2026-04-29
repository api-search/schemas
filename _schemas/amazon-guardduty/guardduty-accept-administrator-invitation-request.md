---
description: AcceptAdministratorInvitationRequest schema from Amazon GuardDuty API
layout: schema
name: AcceptAdministratorInvitationRequest
properties_list:
- description: ''
  name: AdministratorId
  type: object
- description: ''
  name: InvitationId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-accept-administrator-invitation-request-schema.json
slug: guardduty-accept-administrator-invitation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-accept-administrator-invitation-request-schema.json\",\n  \"title\": \"AcceptAdministratorInvitationRequest\",\n  \"description\": \"AcceptAdministratorInvitationRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdministratorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"administratorId\"\n          },\n          \"description\": \"The account ID of the GuardDuty administrator account whose invitation you're accepting.\"\n        }\n      ]\n    },\n    \"InvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitationId\"\
  \n          },\n          \"description\": \"The value that is used to validate the administrator account to the member account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AdministratorId\",\n    \"InvitationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-accept-administrator-invitation-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AcceptAdministratorInvitationRequest
---
