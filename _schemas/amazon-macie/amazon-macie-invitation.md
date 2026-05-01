---
description: Provides information about an Amazon Macie membership invitation.
layout: schema
name: Invitation
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: invitationId
  type: object
- description: ''
  name: invitedAt
  type: object
- description: ''
  name: relationshipStatus
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-invitation-schema.json
slug: amazon-macie-invitation
source_filename: amazon-macie-invitation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-invitation-schema.json\",\n  \"title\": \"Invitation\",\n  \"description\": \"Provides information about an Amazon Macie membership invitation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account that sent the invitation.\"\n        }\n      ]\n    },\n    \"invitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the invitation.\"\n        }\n      ]\n    },\n    \"invitedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\
  \n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the invitation was sent.\"\n        }\n      ]\n    },\n    \"relationshipStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipStatus\"\n        },\n        {\n          \"description\": \"The status of the relationship between the account that sent the invitation and the account that received the invitation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-invitation-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Invitation
---
