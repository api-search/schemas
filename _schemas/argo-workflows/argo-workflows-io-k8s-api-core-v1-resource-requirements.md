---
description: ResourceRequirements describes the compute resource requirements.
layout: schema
name: io.k8s.api.core.v1.ResourceRequirements
properties_list:
- description: 'Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. This field depends on the DynamicResourceAllocation feature gate. This field is immutable. It can '
  name: claims
  type: array
- description: 'Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/'
  name: limits
  type: object
- description: Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defin
  name: requests
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-resource-requirements-schema.json
slug: argo-workflows-io-k8s-api-core-v1-resource-requirements
source_filename: argo-workflows-io-k8s-api-core-v1-resource-requirements-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-resource-requirements-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ResourceRequirements\",\n  \"description\": \"ResourceRequirements describes the compute resource requirements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"claims\": {\n      \"description\": \"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container.\\n\\nThis field depends on the DynamicResourceAllocation feature gate.\\n\\nThis field is immutable. It can only be set for containers.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.ResourceClaim\"\n      },\n      \"x-kubernetes-list-map-keys\": [\n        \"name\"\n      ],\n      \"x-kubernetes-list-type\": \"map\"\n    },\n    \"limits\"\
  : {\n      \"description\": \"Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.api.resource.Quantity\"\n      }\n    },\n    \"requests\": {\n      \"description\": \"Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defined value. Requests cannot exceed Limits. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.api.resource.Quantity\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-resource-requirements-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ResourceRequirements
---
