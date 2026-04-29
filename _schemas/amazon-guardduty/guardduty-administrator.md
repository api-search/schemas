---
description: Contains information about the administrator account and invitation.
layout: schema
name: Administrator
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
schema_file: json-schema/guardduty-administrator-schema.json
slug: guardduty-administrator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-administrator-schema.json\",\n  \"title\": \"Administrator\",\n  \"description\": \"Contains information about the administrator account and invitation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The ID of the account used as the administrator account.\"\n        }\n      ]\n    },\n    \"InvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitationId\"\n          },\n          \"description\": \"The value that is used to validate the administrator\
  \ account to the member account.\"\n        }\n      ]\n    },\n    \"RelationshipStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"relationshipStatus\"\n          },\n          \"description\": \"The status of the relationship between the administrator and member accounts.\"\n        }\n      ]\n    },\n    \"InvitedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitedAt\"\n          },\n          \"description\": \"The timestamp when the invitation was sent.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-administrator-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Administrator
---
