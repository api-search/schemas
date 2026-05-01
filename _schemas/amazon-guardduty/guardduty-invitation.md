---
description: Contains information about the invitation to become a member account.
layout: schema
name: Invitation
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: InvitationId
  type: object
- description: ''
  name: RelationshipStatus
  type: object
- description: ''
  name: InvitedAt
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-invitation-schema.json
slug: guardduty-invitation
source_filename: guardduty-invitation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-invitation-schema.json\",\n  \"title\": \"Invitation\",\n  \"description\": \"Contains information about the invitation to become a member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The ID of the account that the invitation was sent from.\"\n        }\n      ]\n    },\n    \"InvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitationId\"\n          },\n          \"description\": \"The ID of the invitation. This value is used\
  \ to validate the inviter account to the member account.\"\n        }\n      ]\n    },\n    \"RelationshipStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"relationshipStatus\"\n          },\n          \"description\": \"The status of the relationship between the inviter and invitee accounts.\"\n        }\n      ]\n    },\n    \"InvitedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitedAt\"\n          },\n          \"description\": \"The timestamp when the invitation was sent.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-invitation-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Invitation
---
