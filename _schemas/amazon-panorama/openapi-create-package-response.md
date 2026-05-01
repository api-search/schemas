---
description: CreatePackageResponse schema from Amazon Panorama
layout: schema
name: CreatePackageResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: PackageId
  type: object
- description: ''
  name: StorageLocation
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-package-response-schema.json
slug: openapi-create-package-response
source_filename: openapi-create-package-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-response-schema.json\",\n  \"title\": \"CreatePackageResponse\",\n  \"description\": \"CreatePackageResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageArn\"\n        },\n        {\n          \"description\": \"The package's ARN.\"\n        }\n      ]\n    },\n    \"PackageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageId\"\n        },\n        {\n          \"description\": \"The package's ID.\"\n        }\n      ]\n    },\n    \"StorageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageLocation\"\n        },\n        {\n          \"description\": \"The package's\
  \ storage location.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StorageLocation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreatePackageResponse
---
