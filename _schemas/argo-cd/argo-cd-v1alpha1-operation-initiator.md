---
description: v1alpha1OperationInitiator schema from Argo CD API
layout: schema
name: v1alpha1OperationInitiator
properties_list:
- description: Automated is set to true if operation was initiated automatically by the application controller.
  name: automated
  type: boolean
- description: ''
  name: username
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-operation-initiator-schema.json
slug: argo-cd-v1alpha1-operation-initiator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-operation-initiator-schema.json\",\n  \"title\": \"v1alpha1OperationInitiator\",\n  \"description\": \"v1alpha1OperationInitiator schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"automated\": {\n      \"description\": \"Automated is set to true if operation was initiated automatically by the application controller.\",\n      \"type\": \"boolean\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username contains the name of a user who started operation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-operation-initiator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1OperationInitiator
---
