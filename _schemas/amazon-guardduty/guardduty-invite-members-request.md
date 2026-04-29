---
description: InviteMembersRequest schema from Amazon GuardDuty API
layout: schema
name: InviteMembersRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
- description: ''
  name: DisableEmailNotification
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-invite-members-request-schema.json
slug: guardduty-invite-members-request
source_filename: guardduty-invite-members-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-invite-members-request-schema.json\",\n  \"title\": \"InviteMembersRequest\",\n  \"description\": \"InviteMembersRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"A list of account IDs of the accounts that you want to invite to GuardDuty as members.\"\n        }\n      ]\n    },\n    \"DisableEmailNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"disableEmailNotification\"\n          },\n         \
  \ \"description\": \"A Boolean value that specifies whether you want to disable email notification to the accounts that you are inviting to GuardDuty as members.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"message\"\n          },\n          \"description\": \"The invitation message that you want to send to the accounts that you're inviting to GuardDuty as members.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-invite-members-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: InviteMembersRequest
---
