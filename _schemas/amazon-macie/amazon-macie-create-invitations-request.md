---
description: CreateInvitationsRequest schema from Amazon Macie API
layout: schema
name: CreateInvitationsRequest
properties_list:
- description: ''
  name: accountIds
  type: object
- description: ''
  name: disableEmailNotification
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-invitations-request-schema.json
slug: amazon-macie-create-invitations-request
source_filename: amazon-macie-create-invitations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-invitations-request-schema.json\",\n  \"title\": \"CreateInvitationsRequest\",\n  \"description\": \"CreateInvitationsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists Amazon Web Services account IDs, one for each account to send the invitation to.\"\n        }\n      ]\n    },\n    \"disableEmailNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to send the invitation as an email message. If this value is false, Amazon Macie sends the invitation\
  \ (as an email message) to the email address that you specified for the recipient's account when you associated the account with your account. The default value is false.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Custom text to include in the email message that contains the invitation. The text can contain as many as 80 alphanumeric characters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-invitations-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateInvitationsRequest
---
