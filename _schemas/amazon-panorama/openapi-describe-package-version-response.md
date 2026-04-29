---
description: DescribePackageVersionResponse schema from Amazon Panorama
layout: schema
name: DescribePackageVersionResponse
properties_list:
- description: ''
  name: IsLatestPatch
  type: object
- description: ''
  name: OwnerAccount
  type: object
- description: ''
  name: PackageArn
  type: object
- description: ''
  name: PackageId
  type: object
- description: ''
  name: PackageName
  type: object
- description: ''
  name: PackageVersion
  type: object
- description: ''
  name: PatchVersion
  type: object
- description: ''
  name: RegisteredTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusDescription
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-package-version-response-schema.json
slug: openapi-describe-package-version-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-package-version-response-schema.json\",\n  \"title\": \"DescribePackageVersionResponse\",\n  \"description\": \"DescribePackageVersionResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsLatestPatch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the version is the latest available.\"\n        }\n      ]\n    },\n    \"OwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOwnerAccount\"\n        },\n        {\n          \"description\": \"The account ID of the version's owner.\"\n        }\n      ]\n    },\n    \"PackageArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageArn\"\
  \n        },\n        {\n          \"description\": \"The ARN of the package.\"\n        }\n      ]\n    },\n    \"PackageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageId\"\n        },\n        {\n          \"description\": \"The version's ID.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The version's name.\"\n        }\n      ]\n    },\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\": \"The version's version.\"\n        }\n      ]\n    },\n    \"PatchVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackagePatchVersion\"\n        },\n        {\n          \"description\": \"The version's patch version.\"\n        }\n      ]\n\
  \    },\n    \"RegisteredTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"The version's registered time.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \"The version's status.\"\n        }\n      ]\n    },\n    \"StatusDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatusDescription\"\n        },\n        {\n          \"description\": \"The version's status description.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IsLatestPatch\",\n    \"PackageId\",\n    \"PackageName\",\n    \"PackageVersion\",\n    \"PatchVersion\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-package-version-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribePackageVersionResponse
---
