---
description: Paginated list of layer versions
layout: schema
name: ListLayerVersionsResponse
properties_list:
- description: ''
  name: NextMarker
  type: string
- description: ''
  name: LayerVersions
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-list-layer-versions-response-schema.json
slug: aws-lambda-list-layer-versions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListLayerVersionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of layer versions\",\n  \"properties\": {\n    \"NextMarker\": {\n      \"type\": \"string\"\n    },\n    \"LayerVersions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-list-layer-versions-response-schema.json
tags: []
title: ListLayerVersionsResponse
---
