---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: ListVirtualNodesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: virtualNodes
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-list-virtual-nodes-output-schema.json
slug: app-mesh-list-virtual-nodes-output
source_filename: app-mesh-list-virtual-nodes-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>ListVirtualNodes</code> request. When the results of a <code>ListVirtualNodes</code> request exceed <code>limit</code>, you can use this value to retrieve the next page of results. This value is <code>null</code> when there are no more results to return.\"\n        }\n      ]\n    },\n    \"virtualNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeList\"\n        },\n        {\n          \"description\": \"The list of existing virtual nodes for the specified service mesh.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualNodes\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-list-virtual-nodes-output-schema.json\",\n  \"title\": \"ListVirtualNodesOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-list-virtual-nodes-output-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ListVirtualNodesOutput
---
