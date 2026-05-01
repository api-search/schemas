---
description: DeleteInvitationsResponse schema from Amazon Macie API
layout: schema
name: DeleteInvitationsResponse
properties_list:
- description: ''
  name: unprocessedAccounts
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-delete-invitations-response-schema.json
slug: amazon-macie-delete-invitations-response
source_filename: amazon-macie-delete-invitations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-delete-invitations-response-schema.json\",\n  \"title\": \"DeleteInvitationsResponse\",\n  \"description\": \"DeleteInvitationsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unprocessedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUnprocessedAccount\"\n        },\n        {\n          \"description\": \"An array of objects, one for each account whose invitation hasn't been deleted. Each object identifies the account and explains why the request hasn't been processed for that account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-delete-invitations-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DeleteInvitationsResponse
---
