---
description: ListInvitationsResponse schema from Amazon GuardDuty API
layout: schema
name: ListInvitationsResponse
properties_list:
- description: ''
  name: Invitations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-invitations-response-schema.json
slug: guardduty-list-invitations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-invitations-response-schema.json\",\n  \"title\": \"ListInvitationsResponse\",\n  \"description\": \"ListInvitationsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Invitations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Invitations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"invitations\"\n          },\n          \"description\": \"A list of invitation descriptions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The pagination parameter to be used on the next list\
  \ operation to retrieve more items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-invitations-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListInvitationsResponse
---
