---
description: A node instance.
layout: schema
name: NodeInstance
properties_list:
- description: ''
  name: CurrentStatus
  type: object
- description: ''
  name: NodeId
  type: object
- description: ''
  name: NodeInstanceId
  type: object
- description: ''
  name: NodeName
  type: object
- description: ''
  name: PackageName
  type: object
- description: ''
  name: PackagePatchVersion
  type: object
- description: ''
  name: PackageVersion
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-node-instance-schema.json
slug: openapi-node-instance
source_filename: openapi-node-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-instance-schema.json\",\n  \"title\": \"NodeInstance\",\n  \"description\": \"A node instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeInstanceStatus\"\n        },\n        {\n          \"description\": \"The instance's current status.\"\n        }\n      ]\n    },\n    \"NodeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeId\"\n        },\n        {\n          \"description\": \"The node's ID.\"\n        }\n      ]\n    },\n    \"NodeInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeInstanceId\"\n        },\n        {\n          \"description\": \"The instance's ID.\"\n        }\n      ]\n    },\n\
  \    \"NodeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The instance's name.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The instance's package name.\"\n        }\n      ]\n    },\n    \"PackagePatchVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackagePatchVersion\"\n        },\n        {\n          \"description\": \"The instance's package patch version.\"\n        }\n      ]\n    },\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\": \"The instance's package version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentStatus\",\n    \"NodeInstanceId\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-instance-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NodeInstance
---
