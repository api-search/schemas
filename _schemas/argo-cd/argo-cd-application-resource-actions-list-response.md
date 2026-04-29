---
description: applicationResourceActionsListResponse schema from Argo CD API
layout: schema
name: applicationResourceActionsListResponse
properties_list:
- description: ''
  name: actions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-resource-actions-list-response-schema.json
slug: argo-cd-application-resource-actions-list-response
source_filename: argo-cd-application-resource-actions-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-resource-actions-list-response-schema.json\",\n  \"title\": \"applicationResourceActionsListResponse\",\n  \"description\": \"applicationResourceActionsListResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceAction\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-resource-actions-list-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationResourceActionsListResponse
---
