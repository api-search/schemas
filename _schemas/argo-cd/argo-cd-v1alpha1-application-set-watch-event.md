---
description: ApplicationSetWatchEvent contains information about application change.
layout: schema
name: v1alpha1ApplicationSetWatchEvent
properties_list:
- description: ''
  name: applicationSet
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-watch-event-schema.json
slug: argo-cd-v1alpha1-application-set-watch-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-watch-event-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetWatchEvent\",\n  \"description\": \"ApplicationSetWatchEvent contains information about application change.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationSet\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSet\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"Type represents the Kubernetes watch event type. The protobuf tag uses\\ncasttype to ensure the generated Go code keeps this field as\\nwatch.EventType (a strong Go type) instead of falling back to a plain string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-watch-event-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetWatchEvent
---
