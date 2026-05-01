---
description: GetInvitationsCountResponse schema from Amazon Macie API
layout: schema
name: GetInvitationsCountResponse
properties_list:
- description: ''
  name: invitationsCount
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-invitations-count-response-schema.json
slug: amazon-macie-get-invitations-count-response
source_filename: amazon-macie-get-invitations-count-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-invitations-count-response-schema.json\",\n  \"title\": \"GetInvitationsCountResponse\",\n  \"description\": \"GetInvitationsCountResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invitationsCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of invitations that were received by the account, not including the currently accepted invitation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-invitations-count-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetInvitationsCountResponse
---
