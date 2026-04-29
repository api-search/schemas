---
description: v1alpha1ExecProviderConfig schema from Argo CD API
layout: schema
name: v1alpha1ExecProviderConfig
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: args
  type: array
- description: ''
  name: command
  type: string
- description: ''
  name: env
  type: object
- description: ''
  name: installHint
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-exec-provider-config-schema.json
slug: argo-cd-v1alpha1-exec-provider-config
source_filename: argo-cd-v1alpha1-exec-provider-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-exec-provider-config-schema.json\",\n  \"title\": \"v1alpha1ExecProviderConfig\",\n  \"description\": \"v1alpha1ExecProviderConfig schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"title\": \"Preferred input version of the ExecInfo\"\n    },\n    \"args\": {\n      \"type\": \"array\",\n      \"title\": \"Arguments to pass to the command when executing it\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"command\": {\n      \"type\": \"string\",\n      \"title\": \"Command to execute\"\n    },\n    \"env\": {\n      \"type\": \"object\",\n      \"title\": \"Env defines additional environment variables to expose to the process\",\n      \"additionalProperties\": {\n        \"type\": \"\
  string\"\n      }\n    },\n    \"installHint\": {\n      \"type\": \"string\",\n      \"title\": \"This text is shown to the user when the executable doesn't seem to be present\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-exec-provider-config-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ExecProviderConfig
---
