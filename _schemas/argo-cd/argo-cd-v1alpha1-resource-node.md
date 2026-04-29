---
description: ResourceNode contains information about a live Kubernetes resource and its relationships with other resources.
layout: schema
name: v1alpha1ResourceNode
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: health
  type: object
- description: Images lists container images associated with the resource. This is primarily useful for pods and other workload resources.
  name: images
  type: array
- description: Info provides additional metadata or annotations about the resource.
  name: info
  type: array
- description: ''
  name: networkingInfo
  type: object
- description: ParentRefs lists the parent resources that reference this resource. This helps in understanding ownership and hierarchical relationships.
  name: parentRefs
  type: array
- description: ResourceVersion indicates the version of the resource, used to track changes.
  name: resourceVersion
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-node-schema.json
slug: argo-cd-v1alpha1-resource-node
source_filename: argo-cd-v1alpha1-resource-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-node-schema.json\",\n  \"title\": \"v1alpha1ResourceNode\",\n  \"description\": \"ResourceNode contains information about a live Kubernetes resource and its relationships with other resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"health\": {\n      \"$ref\": \"#/definitions/v1alpha1HealthStatus\"\n    },\n    \"images\": {\n      \"description\": \"Images lists container images associated with the resource.\\nThis is primarily useful for pods and other workload resources.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"info\": {\n      \"description\": \"Info provides additional metadata or annotations about the resource.\",\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1InfoItem\"\n      }\n    },\n    \"networkingInfo\": {\n      \"$ref\": \"#/definitions/v1alpha1ResourceNetworkingInfo\"\n    },\n    \"parentRefs\": {\n      \"description\": \"ParentRefs lists the parent resources that reference this resource.\\nThis helps in understanding ownership and hierarchical relationships.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceRef\"\n      }\n    },\n    \"resourceVersion\": {\n      \"description\": \"ResourceVersion indicates the version of the resource, used to track changes.\",\n      \"type\": \"string\"\n    }\n  },\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/v1alpha1ResourceRef\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-node-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceNode
---
