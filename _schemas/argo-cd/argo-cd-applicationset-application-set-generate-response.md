---
description: applicationsetApplicationSetGenerateResponse schema from Argo CD API
layout: schema
name: applicationsetApplicationSetGenerateResponse
properties_list:
- description: ''
  name: applications
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-applicationset-application-set-generate-response-schema.json
slug: argo-cd-applicationset-application-set-generate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationset-application-set-generate-response-schema.json\",\n  \"title\": \"applicationsetApplicationSetGenerateResponse\",\n  \"description\": \"applicationsetApplicationSetGenerateResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Application\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationset-application-set-generate-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationsetApplicationSetGenerateResponse
---
