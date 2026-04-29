---
description: v1alpha1ResourceOverride schema from Argo CD API
layout: schema
name: v1alpha1ResourceOverride
properties_list:
- description: Actions defines the set of actions that can be performed on the resource, as a Lua script.
  name: actions
  type: string
- description: HealthLua contains a Lua script that defines custom health checks for the resource.
  name: healthLua
  type: string
- description: ''
  name: ignoreDifferences
  type: object
- description: ''
  name: ignoreResourceUpdates
  type: object
- description: KnownTypeFields lists fields for which unit conversions should be applied.
  name: knownTypeFields
  type: array
- description: UseOpenLibs indicates whether to use open-source libraries for the resource.
  name: useOpenLibs
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-override-schema.json
slug: argo-cd-v1alpha1-resource-override
source_filename: argo-cd-v1alpha1-resource-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-override-schema.json\",\n  \"title\": \"v1alpha1ResourceOverride\",\n  \"description\": \"v1alpha1ResourceOverride schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"description\": \"Actions defines the set of actions that can be performed on the resource, as a Lua script.\",\n      \"type\": \"string\"\n    },\n    \"healthLua\": {\n      \"description\": \"HealthLua contains a Lua script that defines custom health checks for the resource.\",\n      \"type\": \"string\"\n    },\n    \"ignoreDifferences\": {\n      \"$ref\": \"#/definitions/v1alpha1OverrideIgnoreDiff\"\n    },\n    \"ignoreResourceUpdates\": {\n      \"$ref\": \"#/definitions/v1alpha1OverrideIgnoreDiff\"\n    },\n    \"knownTypeFields\": {\n      \"description\": \"KnownTypeFields\
  \ lists fields for which unit conversions should be applied.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1KnownTypeField\"\n      }\n    },\n    \"useOpenLibs\": {\n      \"description\": \"UseOpenLibs indicates whether to use open-source libraries for the resource.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-override-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceOverride
---
