---
description: Request body for creating a function alias
layout: schema
name: CreateAliasRequest
properties_list:
- description: The name of the alias
  name: Name
  type: string
- description: The function version that the alias invokes
  name: FunctionVersion
  type: string
- description: Description of the alias
  name: Description
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-create-alias-request-schema.json
slug: aws-lambda-create-alias-request
source_filename: aws-lambda-create-alias-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateAliasRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a function alias\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alias\"\n    },\n    \"FunctionVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The function version that the alias invokes\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the alias\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-create-alias-request-schema.json
tags: []
title: CreateAliasRequest
---
