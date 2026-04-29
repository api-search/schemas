---
description: applicationsetApplicationSetResponse schema from Argo CD API
layout: schema
name: applicationsetApplicationSetResponse
properties_list:
- description: ''
  name: applicationset
  type: object
- description: ''
  name: project
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-applicationset-application-set-response-schema.json
slug: argo-cd-applicationset-application-set-response
source_filename: argo-cd-applicationset-application-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationset-application-set-response-schema.json\",\n  \"title\": \"applicationsetApplicationSetResponse\",\n  \"description\": \"applicationsetApplicationSetResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationset\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSet\"\n    },\n    \"project\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationset-application-set-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationsetApplicationSetResponse
---
