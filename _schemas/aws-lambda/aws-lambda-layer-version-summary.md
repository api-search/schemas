---
description: Summary information about a layer version
layout: schema
name: LayerVersionSummary
properties_list:
- description: The ARN of the layer version
  name: LayerVersionArn
  type: string
- description: The version number
  name: Version
  type: integer
- description: Description of the version
  name: Description
  type: string
- description: The date the version was created
  name: CreatedDate
  type: string
- description: ''
  name: CompatibleRuntimes
  type: array
- description: ''
  name: LicenseInfo
  type: string
- description: ''
  name: CompatibleArchitectures
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-layer-version-summary-schema.json
slug: aws-lambda-layer-version-summary
source_filename: aws-lambda-layer-version-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LayerVersionSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary information about a layer version\",\n  \"properties\": {\n    \"LayerVersionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the layer version\"\n    },\n    \"Version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the version\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date the version was created\"\n    },\n    \"CompatibleRuntimes\": {\n      \"type\": \"array\"\n    },\n    \"LicenseInfo\": {\n      \"type\": \"string\"\n    },\n    \"CompatibleArchitectures\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-layer-version-summary-schema.json
tags: []
title: LayerVersionSummary
---
