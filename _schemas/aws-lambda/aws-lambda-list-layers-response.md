---
description: Paginated list of layers
layout: schema
name: ListLayersResponse
properties_list:
- description: ''
  name: NextMarker
  type: string
- description: ''
  name: Layers
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-list-layers-response-schema.json
slug: aws-lambda-list-layers-response
source_filename: aws-lambda-list-layers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListLayersResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of layers\",\n  \"properties\": {\n    \"NextMarker\": {\n      \"type\": \"string\"\n    },\n    \"Layers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-list-layers-response-schema.json
tags: []
title: ListLayersResponse
---
