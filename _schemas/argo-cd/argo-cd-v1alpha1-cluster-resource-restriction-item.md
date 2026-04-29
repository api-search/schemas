---
description: v1alpha1ClusterResourceRestrictionItem schema from Argo CD API
layout: schema
name: v1alpha1ClusterResourceRestrictionItem
properties_list:
- description: ''
  name: group
  type: string
- description: ''
  name: kind
  type: string
- description: Name is the name of the restricted resource. Glob patterns using Go's filepath.Match syntax are supported. Unlike the group and kind fields, if no name is specified, all resources of the specified gro
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-resource-restriction-item-schema.json
slug: argo-cd-v1alpha1-cluster-resource-restriction-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-resource-restriction-item-schema.json\",\n  \"title\": \"v1alpha1ClusterResourceRestrictionItem\",\n  \"description\": \"v1alpha1ClusterResourceRestrictionItem schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name is the name of the restricted resource. Glob patterns using Go's filepath.Match syntax are supported.\\nUnlike the group and kind fields, if no name is specified, all resources of the specified group/kind are matched.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-resource-restriction-item-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterResourceRestrictionItem
---
