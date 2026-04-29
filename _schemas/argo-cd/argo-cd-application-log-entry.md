---
description: applicationLogEntry schema from Argo CD API
layout: schema
name: applicationLogEntry
properties_list:
- description: ''
  name: content
  type: string
- description: ''
  name: last
  type: boolean
- description: ''
  name: podName
  type: string
- description: ''
  name: timeStamp
  type: object
- description: ''
  name: timeStampStr
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-log-entry-schema.json
slug: argo-cd-application-log-entry
source_filename: argo-cd-application-log-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-log-entry-schema.json\",\n  \"title\": \"applicationLogEntry\",\n  \"description\": \"applicationLogEntry schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\"\n    },\n    \"last\": {\n      \"type\": \"boolean\"\n    },\n    \"podName\": {\n      \"type\": \"string\"\n    },\n    \"timeStamp\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"timeStampStr\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-log-entry-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationLogEntry
---
