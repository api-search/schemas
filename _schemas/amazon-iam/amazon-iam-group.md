---
description: Group schema from AWS IAM API
layout: schema
name: Group
properties_list:
- description: The path to the group.
  name: Path
  type: string
- description: The friendly name that identifies the group.
  name: GroupName
  type: string
- description: The stable and unique string identifying the group.
  name: GroupId
  type: string
- description: The Amazon Resource Name (ARN) specifying the group.
  name: Arn
  type: string
- description: The date and time when the group was created.
  name: CreateDate
  type: string
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-group-schema.json
slug: amazon-iam-group
source_filename: amazon-iam-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-group-schema.json\",\n  \"title\": \"Group\",\n  \"description\": \"Group schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the group.\"\n    },\n    \"GroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name that identifies the group.\"\n    },\n    \"GroupId\": {\n      \"type\": \"string\",\n      \"description\": \"The stable and unique string identifying the group.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) specifying the group.\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the group was created.\"\
  \n    }\n  },\n  \"required\": [\n    \"GroupName\",\n    \"GroupId\",\n    \"Arn\",\n    \"CreateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-group-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: Group
---
