---
description: v1alpha1ResourceResult schema from Argo CD API
layout: schema
name: v1alpha1ResourceResult
properties_list:
- description: ''
  name: group
  type: string
- description: HookPhase contains the state of any operation associated with this resource OR hook This can also contain values for non-hook resources.
  name: hookPhase
  type: string
- description: ''
  name: hookType
  type: string
- description: ''
  name: images
  type: array
- description: ''
  name: kind
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: syncPhase
  type: string
- description: ''
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-result-schema.json
slug: argo-cd-v1alpha1-resource-result
source_filename: argo-cd-v1alpha1-resource-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-result-schema.json\",\n  \"title\": \"v1alpha1ResourceResult\",\n  \"description\": \"v1alpha1ResourceResult schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\",\n      \"title\": \"Group specifies the API group of the resource\"\n    },\n    \"hookPhase\": {\n      \"description\": \"HookPhase contains the state of any operation associated with this resource OR hook\\nThis can also contain values for non-hook resources.\",\n      \"type\": \"string\"\n    },\n    \"hookType\": {\n      \"type\": \"string\",\n      \"title\": \"HookType specifies the type of the hook. Empty for non-hook resources\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"title\": \"Images contains the images related to the ResourceResult\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"title\": \"Kind specifies the API kind of the resource\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message contains an informational or error message for the last sync OR operation\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name specifies the name of the resource\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"title\": \"Namespace specifies the target namespace of the resource\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"Status holds the final result of the sync. Will be empty if the resources is yet to be applied/pruned and is always zero-value for hooks\"\n    },\n    \"syncPhase\": {\n      \"type\": \"string\",\n      \"title\": \"SyncPhase indicates the particular phase of the sync that this result was acquired in\"\n    },\n    \"version\"\
  : {\n      \"type\": \"string\",\n      \"title\": \"Version specifies the API version of the resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-result-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceResult
---
