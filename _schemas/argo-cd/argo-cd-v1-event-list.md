---
description: EventList is a list of events.
layout: schema
name: v1EventList
properties_list:
- description: ''
  name: items
  type: array
- description: ''
  name: metadata
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-event-list-schema.json
slug: argo-cd-v1-event-list
source_filename: argo-cd-v1-event-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-list-schema.json\",\n  \"title\": \"v1EventList\",\n  \"description\": \"EventList is a list of events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"title\": \"List of events\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1Event\"\n      }\n    },\n    \"metadata\": {\n      \"$ref\": \"#/definitions/v1ListMeta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-list-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1EventList
---
