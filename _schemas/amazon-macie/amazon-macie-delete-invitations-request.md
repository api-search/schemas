---
description: DeleteInvitationsRequest schema from Amazon Macie API
layout: schema
name: DeleteInvitationsRequest
properties_list:
- description: ''
  name: accountIds
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-delete-invitations-request-schema.json
slug: amazon-macie-delete-invitations-request
source_filename: amazon-macie-delete-invitations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-delete-invitations-request-schema.json\",\n  \"title\": \"DeleteInvitationsRequest\",\n  \"description\": \"DeleteInvitationsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists Amazon Web Services account IDs, one for each account that sent an invitation to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-delete-invitations-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DeleteInvitationsRequest
---
