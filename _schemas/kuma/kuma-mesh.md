---
description: JSON Schema for Kuma service mesh resources including Mesh, Dataplane, and policy types.
layout: schema
name: Kuma Mesh Resource Schema
properties_list:
- description: The Kuma resource type.
  name: type
  type: string
- description: Name of the mesh this resource belongs to.
  name: mesh
  type: string
- description: Name of the resource.
  name: name
  type: string
- description: Time when the resource was created.
  name: creationTime
  type: string
- description: Time when the resource was last modified.
  name: modificationTime
  type: string
- description: Resource labels for grouping and selection.
  name: labels
  type: object
- description: Resource specification, varies by type.
  name: spec
  type: object
- description: Target reference for policies, identifies the resources to which the policy applies.
  name: targetRef
  type: object
- description: Inbound policy rules.
  name: from
  type: array
- description: Outbound policy rules.
  name: to
  type: array
provider_name: Kuma
provider_slug: kuma
schema_file: json-schema/kuma-mesh-schema.json
slug: kuma-mesh
source_filename: kuma-mesh-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/kuma/main/json-schema/kuma-mesh-schema.json\",\n  \"title\": \"Kuma Mesh Resource Schema\",\n  \"description\": \"JSON Schema for Kuma service mesh resources including Mesh, Dataplane, and policy types.\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"name\"],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The Kuma resource type.\",\n      \"enum\": [\n        \"Mesh\",\n        \"Dataplane\",\n        \"DataplaneInsight\",\n        \"ZoneIngress\",\n        \"ZoneEgress\",\n        \"ServiceInsight\",\n        \"MeshTrafficPermission\",\n        \"MeshRetry\",\n        \"MeshTimeout\",\n        \"MeshCircuitBreaker\",\n        \"MeshHealthCheck\",\n        \"MeshFaultInjection\",\n        \"MeshRateLimit\",\n        \"MeshAccessLog\",\n        \"MeshTrace\",\n        \"MeshProxyPatch\",\n \
  \       \"MeshLoadBalancingStrategy\",\n        \"MeshHTTPRoute\",\n        \"MeshTCPRoute\",\n        \"MeshGateway\",\n        \"MeshGatewayRoute\",\n        \"MeshGatewayInstance\"\n      ]\n    },\n    \"mesh\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the mesh this resource belongs to.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the resource.\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time when the resource was created.\"\n    },\n    \"modificationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time when the resource was last modified.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Resource labels for grouping and selection.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"spec\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Resource specification, varies by type.\"\n    },\n    \"targetRef\": {\n      \"type\": \"object\",\n      \"description\": \"Target reference for policies, identifies the resources to which the policy applies.\",\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"enum\": [\"Mesh\", \"MeshSubset\", \"MeshService\", \"MeshServiceSubset\", \"MeshGateway\"]\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"tags\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"from\": {\n      \"type\": \"array\",\n      \"description\": \"Inbound policy rules.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"description\": \"Outbound policy rules.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n \
  \   }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/json-schema/kuma-mesh-schema.json
tags:
- Envoy
- Kubernetes
- Microservices
- Security
- Service Mesh
title: Kuma Mesh Resource Schema
---
