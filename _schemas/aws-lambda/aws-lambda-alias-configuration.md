---
description: Configuration of a Lambda function alias
layout: schema
name: AliasConfiguration
properties_list:
- description: The ARN of the alias
  name: AliasArn
  type: string
- description: The name of the alias
  name: Name
  type: string
- description: The function version that the alias invokes
  name: FunctionVersion
  type: string
- description: Description of the alias
  name: Description
  type: string
- description: A unique identifier that changes when you update the alias
  name: RevisionId
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-alias-configuration-schema.json
slug: aws-lambda-alias-configuration
source_filename: aws-lambda-alias-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AliasConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Configuration of a Lambda function alias\",\n  \"properties\": {\n    \"AliasArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the alias\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alias\"\n    },\n    \"FunctionVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The function version that the alias invokes\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the alias\"\n    },\n    \"RevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier that changes when you update the alias\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-alias-configuration-schema.json
tags: []
title: AliasConfiguration
---
