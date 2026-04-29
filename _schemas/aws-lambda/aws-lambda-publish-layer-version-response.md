---
description: Details about a published layer version
layout: schema
name: PublishLayerVersionResponse
properties_list:
- description: ''
  name: Content
  type: object
- description: The ARN of the layer
  name: LayerArn
  type: string
- description: The ARN of the layer version
  name: LayerVersionArn
  type: string
- description: Description of the version
  name: Description
  type: string
- description: The date the layer version was created in ISO 8601 format
  name: CreatedDate
  type: string
- description: The version number
  name: Version
  type: integer
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
schema_file: json-schema/aws-lambda-publish-layer-version-response-schema.json
slug: aws-lambda-publish-layer-version-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishLayerVersionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Details about a published layer version\",\n  \"properties\": {\n    \"Content\": {\n      \"type\": \"object\"\n    },\n    \"LayerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the layer\"\n    },\n    \"LayerVersionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the layer version\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the version\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date the layer version was created in ISO 8601 format\"\n    },\n    \"Version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number\"\n    },\n    \"CompatibleRuntimes\": {\n      \"type\": \"array\"\n    },\n    \"LicenseInfo\": {\n      \"type\": \"\
  string\"\n    },\n    \"CompatibleArchitectures\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-publish-layer-version-response-schema.json
tags: []
title: PublishLayerVersionResponse
---
