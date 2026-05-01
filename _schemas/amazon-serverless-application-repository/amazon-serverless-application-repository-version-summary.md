---
description: Summary of details about an application version.
layout: schema
name: VersionSummary
properties_list:
- description: The application ARN.
  name: applicationId
  type: string
- description: The semantic version of the application.
  name: semanticVersion
  type: string
- description: The date and time when this version was created.
  name: creationTime
  type: string
- description: A link to a public repository for the source code.
  name: sourceCodeUrl
  type: string
provider_name: Amazon Serverless Application Repository
provider_slug: amazon-serverless-application-repository
schema_file: json-schema/amazon-serverless-application-repository-version-summary-schema.json
slug: amazon-serverless-application-repository-version-summary
source_filename: amazon-serverless-application-repository-version-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-version-summary-schema.json\",\n  \"title\": \"VersionSummary\",\n  \"description\": \"Summary of details about an application version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application ARN.\",\n      \"example\": \"arn:aws:serverlessrepo:us-east-1:123456789012:applications/MyApp\"\n    },\n    \"semanticVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The semantic version of the application.\",\n      \"example\": \"1.0.0\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when this version was created.\"\n    },\n    \"sourceCodeUrl\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"A link to a public repository for the source code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-version-summary-schema.json
tags:
- Application Repository
- Lambda
- SAM
- Serverless
title: VersionSummary
---
