---
description: applicationApplicationRollbackRequest schema from Argo CD API
layout: schema
name: applicationApplicationRollbackRequest
properties_list:
- description: ''
  name: appNamespace
  type: string
- description: ''
  name: dryRun
  type: boolean
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: project
  type: string
- description: ''
  name: prune
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-application-rollback-request-schema.json
slug: argo-cd-application-application-rollback-request
source_filename: argo-cd-application-application-rollback-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-rollback-request-schema.json\",\n  \"title\": \"applicationApplicationRollbackRequest\",\n  \"description\": \"applicationApplicationRollbackRequest schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appNamespace\": {\n      \"type\": \"string\"\n    },\n    \"dryRun\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"project\": {\n      \"type\": \"string\"\n    },\n    \"prune\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-rollback-request-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationApplicationRollbackRequest
---
