---
description: ApplicationWatchEvent contains information about application change.
layout: schema
name: v1alpha1ApplicationWatchEvent
properties_list:
- description: ''
  name: application
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-watch-event-schema.json
slug: argo-cd-v1alpha1-application-watch-event
source_filename: argo-cd-v1alpha1-application-watch-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-watch-event-schema.json\",\n  \"title\": \"v1alpha1ApplicationWatchEvent\",\n  \"description\": \"ApplicationWatchEvent contains information about application change.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"$ref\": \"#/definitions/v1alpha1Application\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-watch-event-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationWatchEvent
---
