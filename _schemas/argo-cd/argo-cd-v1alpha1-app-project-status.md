---
description: v1alpha1AppProjectStatus schema from Argo CD API
layout: schema
name: v1alpha1AppProjectStatus
properties_list:
- description: ''
  name: jwtTokensByRole
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-app-project-status-schema.json
slug: argo-cd-v1alpha1-app-project-status
source_filename: argo-cd-v1alpha1-app-project-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-status-schema.json\",\n  \"title\": \"v1alpha1AppProjectStatus\",\n  \"description\": \"v1alpha1AppProjectStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jwtTokensByRole\": {\n      \"type\": \"object\",\n      \"title\": \"JWTTokensByRole contains a list of JWT tokens issued for a given role\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/v1alpha1JWTTokens\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1AppProjectStatus
---
