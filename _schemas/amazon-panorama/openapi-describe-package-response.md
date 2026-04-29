---
description: DescribePackageResponse schema from Amazon Panorama
layout: schema
name: DescribePackageResponse
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
  name: ReadAccessPrincipalArns
  type: object
- description: ''
  name: StorageLocation
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: WriteAccessPrincipalArns
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-package-response-schema.json
slug: openapi-describe-package-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-package-response-schema.json\",\n  \"title\": \"DescribePackageResponse\",\n  \"description\": \"DescribePackageResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageArn\"\n        },\n        {\n          \"description\": \"The package's ARN.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"When the package was created.\"\n        }\n      ]\n    },\n    \"PackageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageId\"\n        },\n        {\n          \"description\":\
  \ \"The package's ID.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The package's name.\"\n        }\n      ]\n    },\n    \"ReadAccessPrincipalArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalArnsList\"\n        },\n        {\n          \"description\": \"ARNs of accounts that have read access to the package.\"\n        }\n      ]\n    },\n    \"StorageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageLocation\"\n        },\n        {\n          \"description\": \"The package's storage location.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The package's tags.\"\n        }\n      ]\n    },\n    \"WriteAccessPrincipalArns\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalArnsList\"\n        },\n        {\n          \"description\": \"ARNs of accounts that have write access to the package.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"CreatedTime\",\n    \"PackageId\",\n    \"PackageName\",\n    \"StorageLocation\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-package-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribePackageResponse
---
