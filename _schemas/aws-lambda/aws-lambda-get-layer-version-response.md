---
description: Details about a layer version
layout: schema
name: GetLayerVersionResponse
properties_list:
- description: ''
  name: Content
  type: object
- description: ''
  name: LayerArn
  type: string
- description: ''
  name: LayerVersionArn
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: CreatedDate
  type: string
- description: ''
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
schema_file: json-schema/aws-lambda-get-layer-version-response-schema.json
slug: aws-lambda-get-layer-version-response
source_filename: aws-lambda-get-layer-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetLayerVersionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Details about a layer version\",\n  \"properties\": {\n    \"Content\": {\n      \"type\": \"object\"\n    },\n    \"LayerArn\": {\n      \"type\": \"string\"\n    },\n    \"LayerVersionArn\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\"\n    },\n    \"Version\": {\n      \"type\": \"integer\"\n    },\n    \"CompatibleRuntimes\": {\n      \"type\": \"array\"\n    },\n    \"LicenseInfo\": {\n      \"type\": \"string\"\n    },\n    \"CompatibleArchitectures\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-get-layer-version-response-schema.json
tags: []
title: GetLayerVersionResponse
---
