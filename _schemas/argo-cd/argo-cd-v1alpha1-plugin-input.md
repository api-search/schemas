---
description: v1alpha1PluginInput schema from Argo CD API
layout: schema
name: v1alpha1PluginInput
properties_list:
- description: Parameters contains the information to pass to the plugin. It is a map. The keys must be strings, and the values can be any type.
  name: parameters
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-plugin-input-schema.json
slug: argo-cd-v1alpha1-plugin-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-plugin-input-schema.json\",\n  \"title\": \"v1alpha1PluginInput\",\n  \"description\": \"v1alpha1PluginInput schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"description\": \"Parameters contains the information to pass to the plugin. It is a map. The keys must be strings, and the\\nvalues can be any type.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/v1JSON\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-plugin-input-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PluginInput
---
