---
description: Request body for updating a function alias
layout: schema
name: UpdateAliasRequest
properties_list:
- description: The function version that the alias invokes
  name: FunctionVersion
  type: string
- description: Description of the alias
  name: Description
  type: string
- description: Update only if the revision ID matches
  name: RevisionId
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-update-alias-request-schema.json
slug: aws-lambda-update-alias-request
source_filename: aws-lambda-update-alias-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateAliasRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a function alias\",\n  \"properties\": {\n    \"FunctionVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The function version that the alias invokes\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the alias\"\n    },\n    \"RevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Update only if the revision ID matches\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-update-alias-request-schema.json
tags: []
title: UpdateAliasRequest
---
