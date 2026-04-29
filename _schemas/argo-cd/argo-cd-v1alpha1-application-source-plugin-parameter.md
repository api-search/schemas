---
description: v1alpha1ApplicationSourcePluginParameter schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourcePluginParameter
properties_list:
- description: Array is the value of an array type parameter.
  name: array
  type: array
- description: Map is the value of a map type parameter.
  name: map
  type: object
- description: Name is the name identifying a parameter.
  name: name
  type: string
- description: String_ is the value of a string type parameter.
  name: string
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-plugin-parameter-schema.json
slug: argo-cd-v1alpha1-application-source-plugin-parameter
source_filename: argo-cd-v1alpha1-application-source-plugin-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-plugin-parameter-schema.json\",\n  \"title\": \"v1alpha1ApplicationSourcePluginParameter\",\n  \"description\": \"v1alpha1ApplicationSourcePluginParameter schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"array\": {\n      \"description\": \"Array is the value of an array type parameter.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"map\": {\n      \"description\": \"Map is the value of a map type parameter.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"description\": \"Name is the name identifying a parameter.\",\n      \"type\": \"string\"\n    },\n    \"string\": {\n      \"description\": \"\
  String_ is the value of a string type parameter.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-plugin-parameter-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourcePluginParameter
---
