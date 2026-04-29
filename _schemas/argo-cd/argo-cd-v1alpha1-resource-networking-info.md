---
description: ResourceNetworkingInfo holds networking-related information for a resource.
layout: schema
name: v1alpha1ResourceNetworkingInfo
properties_list:
- description: ExternalURLs holds a list of URLs that should be accessible externally. This field is typically populated for Ingress resources based on their hostname rules.
  name: externalURLs
  type: array
- description: Ingress provides information about external access points (e.g., load balancer ingress) for this resource.
  name: ingress
  type: array
- description: Labels holds the labels associated with this networking resource.
  name: labels
  type: object
- description: TargetLabels represents labels associated with the target resources that this resource communicates with.
  name: targetLabels
  type: object
- description: TargetRefs contains references to other resources that this resource interacts with, such as Services or Pods.
  name: targetRefs
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-networking-info-schema.json
slug: argo-cd-v1alpha1-resource-networking-info
source_filename: argo-cd-v1alpha1-resource-networking-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-networking-info-schema.json\",\n  \"title\": \"v1alpha1ResourceNetworkingInfo\",\n  \"description\": \"ResourceNetworkingInfo holds networking-related information for a resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalURLs\": {\n      \"description\": \"ExternalURLs holds a list of URLs that should be accessible externally.\\nThis field is typically populated for Ingress resources based on their hostname rules.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ingress\": {\n      \"description\": \"Ingress provides information about external access points (e.g., load balancer ingress) for this resource.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1LoadBalancerIngress\"\
  \n      }\n    },\n    \"labels\": {\n      \"description\": \"Labels holds the labels associated with this networking resource.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"targetLabels\": {\n      \"description\": \"TargetLabels represents labels associated with the target resources that this resource communicates with.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"targetRefs\": {\n      \"description\": \"TargetRefs contains references to other resources that this resource interacts with, such as Services or Pods.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceRef\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-networking-info-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceNetworkingInfo
---
