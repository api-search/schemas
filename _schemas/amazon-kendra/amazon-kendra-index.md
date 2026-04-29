---
description: An Amazon Kendra search index.
layout: schema
name: Index
properties_list:
- description: The unique identifier of the index.
  name: Id
  type: string
- description: The name of the index.
  name: Name
  type: string
- description: The current status of the index.
  name: Status
  type: string
- description: The Amazon Kendra edition.
  name: Edition
  type: string
- description: The IAM role ARN for the index.
  name: RoleArn
  type: string
- description: When the index was created.
  name: CreatedAt
  type: string
- description: When the index was last updated.
  name: UpdatedAt
  type: string
provider_name: Amazon Kendra
provider_slug: amazon-kendra
schema_file: json-schema/amazon-kendra-index-schema.json
slug: amazon-kendra-index
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-index-schema.json\",\n  \"title\": \"Index\",\n  \"description\": \"An Amazon Kendra search index.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the index.\",\n      \"example\": \"abc12345-6789-def0-1234-abcdef012345\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the index.\",\n      \"example\": \"my-enterprise-index\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"FAILED\",\n        \"UPDATING\",\n        \"SYSTEM_UPDATING\"\n      ],\n      \"description\": \"The current status of the index.\",\n      \"example\": \"ACTIVE\"\n    },\n    \"\
  Edition\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DEVELOPER_EDITION\",\n        \"ENTERPRISE_EDITION\",\n        \"GEN_AI_ENTERPRISE_EDITION\"\n      ],\n      \"description\": \"The Amazon Kendra edition.\",\n      \"example\": \"ENTERPRISE_EDITION\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The IAM role ARN for the index.\",\n      \"example\": \"arn:aws:iam::123456789012:role/KendraRole\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the index was created.\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the index was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-index-schema.json
tags:
- AI
- AWS
- Enterprise Search
- Knowledge Management
- Machine Learning
- Natural Language
title: Index
---
