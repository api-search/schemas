---
description: Policy statement for an application.
layout: schema
name: ApplicationPolicyStatement
properties_list:
- description: A unique ID for the statement.
  name: statementId
  type: string
- description: An array of AWS account IDs or * for public access.
  name: principals
  type: array
- description: For each action, specify the permission to be granted.
  name: actions
  type: array
provider_name: Amazon Serverless Application Repository
provider_slug: amazon-serverless-application-repository
schema_file: json-schema/amazon-serverless-application-repository-application-policy-statement-schema.json
slug: amazon-serverless-application-repository-application-policy-statement
source_filename: amazon-serverless-application-repository-application-policy-statement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-application-policy-statement-schema.json\",\n  \"title\": \"ApplicationPolicyStatement\",\n  \"description\": \"Policy statement for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statementId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique ID for the statement.\",\n      \"example\": \"policy-stmt-001\"\n    },\n    \"principals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"An array of AWS account IDs or * for public access.\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"For each action, specify the permission to be granted.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-application-policy-statement-schema.json
tags:
- Application Repository
- Lambda
- SAM
- Serverless
title: ApplicationPolicyStatement
---
