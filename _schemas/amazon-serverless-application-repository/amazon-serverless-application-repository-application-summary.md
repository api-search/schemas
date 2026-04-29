---
description: Summary of details about the application.
layout: schema
name: ApplicationSummary
properties_list:
- description: The application ARN.
  name: applicationId
  type: string
- description: The name of the application.
  name: name
  type: string
- description: The name of the author.
  name: author
  type: string
- description: The description of the application.
  name: description
  type: string
- description: The date and time when created.
  name: creationTime
  type: string
- description: Labels for discovery.
  name: labels
  type: array
provider_name: Amazon Serverless Application Repository
provider_slug: amazon-serverless-application-repository
schema_file: json-schema/amazon-serverless-application-repository-application-summary-schema.json
slug: amazon-serverless-application-repository-application-summary
source_filename: amazon-serverless-application-repository-application-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-application-summary-schema.json\",\n  \"title\": \"ApplicationSummary\",\n  \"description\": \"Summary of details about the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application ARN.\",\n      \"example\": \"arn:aws:serverlessrepo:us-east-1:123456789012:applications/MyApp\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\",\n      \"example\": \"MyApp\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the author.\",\n      \"example\": \"developer@example.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The description of the application.\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when created.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels for discovery.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-application-summary-schema.json
tags:
- Application Repository
- AWS
- Lambda
- SAM
- Serverless
title: ApplicationSummary
---
