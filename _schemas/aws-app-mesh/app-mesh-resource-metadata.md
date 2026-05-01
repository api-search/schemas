---
description: An object that represents metadata for a resource.
layout: schema
name: ResourceMetadata
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: meshOwner
  type: object
- description: ''
  name: resourceOwner
  type: object
- description: ''
  name: uid
  type: object
- description: ''
  name: version
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-resource-metadata-schema.json
slug: app-mesh-resource-metadata
source_filename: app-mesh-resource-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The full Amazon Resource Name (ARN) for the resource.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The Unix epoch timestamp in seconds for when the resource was created.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The Unix epoch timestamp in seconds for when the resource was last updated.\"\n        }\n      ]\n    },\n    \"meshOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon\
  \ Web Services IAM account ID of the service mesh owner. If the account ID is not your own, then it's the ID of the account that shared the mesh with your account. For more information about mesh sharing, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/sharing.html\\\">Working with shared meshes</a>.\"\n        }\n      ]\n    },\n    \"resourceOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services IAM account ID of the resource owner. If the account ID is not your own, then it's the ID of the mesh owner or of another account that the mesh is shared with. For more information about mesh sharing, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/sharing.html\\\">Working with shared meshes</a>.\"\n        }\n      ]\n    },\n    \"uid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n    \
  \    },\n        {\n          \"description\": \"The unique identifier for the resource.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The version of the resource. Resources are created at version 1, and this version is incremented each time that they're updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastUpdatedAt\",\n    \"meshOwner\",\n    \"resourceOwner\",\n    \"uid\",\n    \"version\"\n  ],\n  \"description\": \"An object that represents metadata for a resource.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-resource-metadata-schema.json\",\n  \"title\": \"ResourceMetadata\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-resource-metadata-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ResourceMetadata
---
