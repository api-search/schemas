---
description: PluginGenerator defines connection info specific to Plugin.
layout: schema
name: v1alpha1PluginGenerator
properties_list:
- description: ''
  name: configMapRef
  type: object
- description: ''
  name: input
  type: object
- description: RequeueAfterSeconds determines how long the ApplicationSet controller will wait before reconciling the ApplicationSet again.
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: template
  type: object
- description: Values contains key/value pairs which are passed directly as parameters to the template. These values will not be sent as parameters to the plugin.
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-plugin-generator-schema.json
slug: argo-cd-v1alpha1-plugin-generator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-plugin-generator-schema.json\",\n  \"title\": \"v1alpha1PluginGenerator\",\n  \"description\": \"PluginGenerator defines connection info specific to Plugin.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapRef\": {\n      \"$ref\": \"#/definitions/v1alpha1PluginConfigMapRef\"\n    },\n    \"input\": {\n      \"$ref\": \"#/definitions/v1alpha1PluginInput\"\n    },\n    \"requeueAfterSeconds\": {\n      \"description\": \"RequeueAfterSeconds determines how long the ApplicationSet controller will wait before reconciling the ApplicationSet again.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"values\": {\n      \"description\": \"Values contains key/value pairs\
  \ which are passed directly as parameters to the template. These values will not be\\nsent as parameters to the plugin.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-plugin-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PluginGenerator
---
