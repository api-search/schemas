---
description: An observed connection edge between two meshed Kubernetes resources, including mTLS identity information.
layout: schema
name: Linkerd Edge
properties_list:
- description: Source resource of the connection.
  name: src
  type: object
- description: Destination resource of the connection.
  name: dst
  type: object
- description: TLS client identity of the source.
  name: client_id
  type: string
- description: TLS server identity of the destination.
  name: server_id
  type: string
- description: Reason for missing mTLS identity, if applicable.
  name: no_identity_msg
  type: string
provider_name: Linkerd
provider_slug: linkerd
schema_file: json-schema/edge.json
slug: edge
source_filename: edge.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/linkerd/blob/main/json-schema/edge.json\",\n  \"title\": \"Linkerd Edge\",\n  \"description\": \"An observed connection edge between two meshed Kubernetes resources, including mTLS identity information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"src\": {\n      \"$ref\": \"#/$defs/Resource\",\n      \"description\": \"Source resource of the connection.\"\n    },\n    \"dst\": {\n      \"$ref\": \"#/$defs/Resource\",\n      \"description\": \"Destination resource of the connection.\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"TLS client identity of the source.\"\n    },\n    \"server_id\": {\n      \"type\": \"string\",\n      \"description\": \"TLS server identity of the destination.\"\n    },\n    \"no_identity_msg\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for missing mTLS identity,\
  \ if applicable.\"\n    }\n  },\n  \"$defs\": {\n    \"Resource\": {\n      \"type\": \"object\",\n      \"description\": \"A Kubernetes resource reference.\",\n      \"properties\": {\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Resource type (e.g., deployment, pod, service).\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/json-schema/edge.json
tags:
- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh
title: Linkerd Edge
---
