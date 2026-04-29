---
description: UpdateMemberSessionRequest schema from Amazon Macie API
layout: schema
name: UpdateMemberSessionRequest
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-member-session-request-schema.json
slug: amazon-macie-update-member-session-request
source_filename: amazon-macie-update-member-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-member-session-request-schema.json\",\n  \"title\": \"UpdateMemberSessionRequest\",\n  \"description\": \"UpdateMemberSessionRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacieStatus\"\n        },\n        {\n          \"description\": \"Specifies the new status for the account. Valid values are: ENABLED, resume all Amazon Macie activities for the account; and, PAUSED, suspend all Macie activities for the account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-member-session-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateMemberSessionRequest
---
