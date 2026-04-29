---
description: HostInfo holds metadata and resource usage metrics for a specific host in the cluster.
layout: schema
name: v1alpha1HostInfo
properties_list:
- description: Labels holds the labels attached to the host.
  name: labels
  type: object
- description: Name is the hostname or node name in the Kubernetes cluster.
  name: name
  type: string
- description: ResourcesInfo provides a list of resource usage details for different resource types on this host.
  name: resourcesInfo
  type: array
- description: ''
  name: systemInfo
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-host-info-schema.json
slug: argo-cd-v1alpha1-host-info
source_filename: argo-cd-v1alpha1-host-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-host-info-schema.json\",\n  \"title\": \"v1alpha1HostInfo\",\n  \"description\": \"HostInfo holds metadata and resource usage metrics for a specific host in the cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"labels\": {\n      \"description\": \"Labels holds the labels attached to the host.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"description\": \"Name is the hostname or node name in the Kubernetes cluster.\",\n      \"type\": \"string\"\n    },\n    \"resourcesInfo\": {\n      \"description\": \"ResourcesInfo provides a list of resource usage details for different resource types on this host.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1HostResourceInfo\"\
  \n      }\n    },\n    \"systemInfo\": {\n      \"$ref\": \"#/definitions/v1NodeSystemInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-host-info-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HostInfo
---
