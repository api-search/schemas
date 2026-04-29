---
description: v1alpha1ApplicationSetCondition schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetCondition
properties_list:
- description: ''
  name: lastTransitionTime
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: reason
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-condition-schema.json
slug: argo-cd-v1alpha1-application-set-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-condition-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetCondition\",\n  \"description\": \"v1alpha1ApplicationSetCondition schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastTransitionTime\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message contains human-readable message indicating details about condition\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"title\": \"Single word camelcase representing the reason for the status eg ErrorOccurred\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"True/False/Unknown\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"Type is an applicationset condition\
  \ type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-condition-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetCondition
---
