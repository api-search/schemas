---
description: v1alpha1ApplicationSourcePlugin schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourcePlugin
properties_list:
- description: ''
  name: env
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: parameters
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-plugin-schema.json
slug: argo-cd-v1alpha1-application-source-plugin
source_filename: argo-cd-v1alpha1-application-source-plugin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-plugin-schema.json\",\n  \"title\": \"v1alpha1ApplicationSourcePlugin\",\n  \"description\": \"v1alpha1ApplicationSourcePlugin schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"env\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/applicationv1alpha1EnvEntry\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSourcePluginParameter\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-plugin-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourcePlugin
---
