---
description: v1alpha1HealthStatus schema from Argo CD API
layout: schema
name: v1alpha1HealthStatus
properties_list:
- description: ''
  name: lastTransitionTime
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: status
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-health-status-schema.json
slug: argo-cd-v1alpha1-health-status
source_filename: argo-cd-v1alpha1-health-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-health-status-schema.json\",\n  \"title\": \"v1alpha1HealthStatus\",\n  \"description\": \"v1alpha1HealthStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastTransitionTime\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message is a human-readable informational message describing the health status\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"Status holds the status code of the resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-health-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HealthStatus
---
