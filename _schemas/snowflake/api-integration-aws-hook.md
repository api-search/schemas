---
description: ''
layout: schema
name: AwsHook
properties_list:
- description: ''
  name: api_provider
  type: string
- description: The ARN (Amazon resource name) of the IAM role.
  name: api_aws_role_arn
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/api-integration-aws-hook-schema.json
slug: api-integration-aws-hook
source_filename: api-integration-aws-hook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AwsHook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_provider\": {\n      \"type\": \"string\"\n    },\n    \"api_aws_role_arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN (Amazon resource name) of the IAM role.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/api-integration-aws-hook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: AwsHook
---
