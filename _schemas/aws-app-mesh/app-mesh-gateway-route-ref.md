---
description: An object that represents a gateway route returned by a list operation.
layout: schema
name: GatewayRouteRef
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: gatewayRouteName
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: meshName
  type: object
- description: ''
  name: meshOwner
  type: object
- description: ''
  name: resourceOwner
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: virtualGatewayName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-ref-schema.json
slug: app-mesh-gateway-route-ref
source_filename: app-mesh-gateway-route-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The full Amazon Resource Name (ARN) for the gateway route.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The Unix epoch timestamp in seconds for when the resource was created.\"\n        }\n      ]\n    },\n    \"gatewayRouteName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the gateway route.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The Unix epoch timestamp in seconds for\
  \ when the resource was last updated.\"\n        }\n      ]\n    },\n    \"meshName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service mesh that the resource resides in. \"\n        }\n      ]\n    },\n    \"meshOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services IAM account ID of the service mesh owner. If the account ID is not your own, then it's the ID of the account that shared the mesh with your account. For more information about mesh sharing, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/sharing.html\\\">Working with shared meshes</a>.\"\n        }\n      ]\n    },\n    \"resourceOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\"\
  : \"The Amazon Web Services IAM account ID of the resource owner. If the account ID is not your own, then it's the ID of the mesh owner or of another account that the mesh is shared with. For more information about mesh sharing, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/sharing.html\\\">Working with shared meshes</a>.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The version of the resource. Resources are created at version 1, and this version is incremented each time that they're updated.\"\n        }\n      ]\n    },\n    \"virtualGatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The virtual gateway that the gateway route is associated with.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n \
  \   \"createdAt\",\n    \"gatewayRouteName\",\n    \"lastUpdatedAt\",\n    \"meshName\",\n    \"meshOwner\",\n    \"resourceOwner\",\n    \"version\",\n    \"virtualGatewayName\"\n  ],\n  \"description\": \"An object that represents a gateway route returned by a list operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-ref-schema.json\",\n  \"title\": \"GatewayRouteRef\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-ref-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteRef
---
