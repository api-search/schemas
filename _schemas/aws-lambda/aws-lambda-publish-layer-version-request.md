---
description: Request body for publishing a layer version
layout: schema
name: PublishLayerVersionRequest
properties_list:
- description: Description of the layer version
  name: Description
  type: string
- description: The function layer archive
  name: Content
  type: object
- description: A list of compatible runtimes. Used for filtering with ListLayers and ListLayerVersions.
  name: CompatibleRuntimes
  type: array
- description: The layer's software license (SPDX identifier, URL, or text)
  name: LicenseInfo
  type: string
- description: A list of compatible instruction set architectures
  name: CompatibleArchitectures
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-publish-layer-version-request-schema.json
slug: aws-lambda-publish-layer-version-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishLayerVersionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for publishing a layer version\",\n  \"properties\": {\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the layer version\"\n    },\n    \"Content\": {\n      \"type\": \"object\",\n      \"description\": \"The function layer archive\"\n    },\n    \"CompatibleRuntimes\": {\n      \"type\": \"array\",\n      \"description\": \"A list of compatible runtimes. Used for filtering with ListLayers and ListLayerVersions.\"\n    },\n    \"LicenseInfo\": {\n      \"type\": \"string\",\n      \"description\": \"The layer's software license (SPDX identifier, URL, or text)\"\n    },\n    \"CompatibleArchitectures\": {\n      \"type\": \"array\",\n      \"description\": \"A list of compatible instruction set architectures\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-publish-layer-version-request-schema.json
tags: []
title: PublishLayerVersionRequest
---
