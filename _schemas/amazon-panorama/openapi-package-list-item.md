---
description: A package summary.
layout: schema
name: PackageListItem
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: PackageId
  type: object
- description: ''
  name: PackageName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-list-item-schema.json
slug: openapi-package-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-list-item-schema.json\",\n  \"title\": \"PackageListItem\",\n  \"description\": \"A package summary.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageArn\"\n        },\n        {\n          \"description\": \"The package's ARN.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"When the package was created.\"\n        }\n      ]\n    },\n    \"PackageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageId\"\n        },\n        {\n          \"description\": \"The package's ID.\"\n        }\n      ]\n    },\n\
  \    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The package's name.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The package's tags.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-list-item-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageListItem
---
