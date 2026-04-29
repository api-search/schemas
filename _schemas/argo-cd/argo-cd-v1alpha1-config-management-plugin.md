---
description: v1alpha1ConfigManagementPlugin schema from Argo CD API
layout: schema
name: v1alpha1ConfigManagementPlugin
properties_list:
- description: ''
  name: generate
  type: object
- description: ''
  name: init
  type: object
- description: ''
  name: lockRepo
  type: boolean
- description: ''
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-config-management-plugin-schema.json
slug: argo-cd-v1alpha1-config-management-plugin
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-config-management-plugin-schema.json\",\n  \"title\": \"v1alpha1ConfigManagementPlugin\",\n  \"description\": \"v1alpha1ConfigManagementPlugin schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"generate\": {\n      \"$ref\": \"#/definitions/v1alpha1Command\"\n    },\n    \"init\": {\n      \"$ref\": \"#/definitions/v1alpha1Command\"\n    },\n    \"lockRepo\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-config-management-plugin-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ConfigManagementPlugin
---
