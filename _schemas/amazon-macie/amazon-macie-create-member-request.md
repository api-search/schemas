---
description: CreateMemberRequest schema from Amazon Macie API
layout: schema
name: CreateMemberRequest
properties_list:
- description: ''
  name: account
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-member-request-schema.json
slug: amazon-macie-create-member-request
source_filename: amazon-macie-create-member-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-member-request-schema.json\",\n  \"title\": \"CreateMemberRequest\",\n  \"description\": \"CreateMemberRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountDetail\"\n        },\n        {\n          \"description\": \"The details of the account to associate with the administrator account.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>A map of key-value pairs that specifies the tags to associate with the account in Amazon Macie.</p> <p>An account can have a maximum of 50 tags. Each tag consists of a tag key and an associated\
  \ tag value. The maximum length of a tag key is 128 characters. The maximum length of a tag value is 256 characters.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"account\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-member-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateMemberRequest
---
