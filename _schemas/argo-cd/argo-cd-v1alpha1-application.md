---
description: v1alpha1Application schema from Argo CD API
layout: schema
name: v1alpha1Application
properties_list:
- description: ''
  name: metadata
  type: object
- description: ''
  name: operation
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-schema.json
slug: argo-cd-v1alpha1-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-schema.json\",\n  \"title\": \"v1alpha1Application\",\n  \"description\": \"v1alpha1Application schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"#/definitions/v1ObjectMeta\"\n    },\n    \"operation\": {\n      \"$ref\": \"#/definitions/v1alpha1Operation\"\n    },\n    \"spec\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSpec\"\n    },\n    \"status\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1Application
---
