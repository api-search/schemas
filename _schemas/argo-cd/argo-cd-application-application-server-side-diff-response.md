---
description: applicationApplicationServerSideDiffResponse schema from Argo CD API
layout: schema
name: applicationApplicationServerSideDiffResponse
properties_list:
- description: ''
  name: items
  type: array
- description: ''
  name: modified
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-application-server-side-diff-response-schema.json
slug: argo-cd-application-application-server-side-diff-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-server-side-diff-response-schema.json\",\n  \"title\": \"applicationApplicationServerSideDiffResponse\",\n  \"description\": \"applicationApplicationServerSideDiffResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceDiff\"\n      }\n    },\n    \"modified\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-server-side-diff-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationApplicationServerSideDiffResponse
---
