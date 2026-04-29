---
description: DescribeNodeResponse schema from Amazon Panorama
layout: schema
name: DescribeNodeResponse
properties_list:
- description: ''
  name: AssetName
  type: object
- description: ''
  name: Category
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: NodeId
  type: object
- description: ''
  name: NodeInterface
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
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-node-response-schema.json
slug: openapi-describe-node-response
source_filename: openapi-describe-node-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-node-response-schema.json\",\n  \"title\": \"DescribeNodeResponse\",\n  \"description\": \"DescribeNodeResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeAssetName\"\n        },\n        {\n          \"description\": \"The node's asset name.\"\n        }\n      ]\n    },\n    \"Category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeCategory\"\n        },\n        {\n          \"description\": \"The node's category.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"When the\
  \ node was created.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The node's description.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"When the node was updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The node's name.\"\n        }\n      ]\n    },\n    \"NodeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeId\"\n        },\n        {\n          \"description\": \"The node's ID.\"\n        }\n      ]\n    },\n    \"NodeInterface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeInterface\"\
  \n        },\n        {\n          \"description\": \"The node's interface.\"\n        }\n      ]\n    },\n    \"OwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOwnerAccount\"\n        },\n        {\n          \"description\": \"The account ID of the node's owner.\"\n        }\n      ]\n    },\n    \"PackageArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageArn\"\n        },\n        {\n          \"description\": \"The node's ARN.\"\n        }\n      ]\n    },\n    \"PackageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageId\"\n        },\n        {\n          \"description\": \"The node's package ID.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The node's package name.\"\n        }\n      ]\n \
  \   },\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\": \"The node's package version.\"\n        }\n      ]\n    },\n    \"PatchVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackagePatchVersion\"\n        },\n        {\n          \"description\": \"The node's patch version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Category\",\n    \"CreatedTime\",\n    \"Description\",\n    \"LastUpdatedTime\",\n    \"Name\",\n    \"NodeId\",\n    \"NodeInterface\",\n    \"OwnerAccount\",\n    \"PackageId\",\n    \"PackageName\",\n    \"PackageVersion\",\n    \"PatchVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-node-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribeNodeResponse
---
