---
description: EventSeries contain information on series of events, i.e. thing that was/is happening continuously for some time.
layout: schema
name: v1EventSeries
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: lastObservedTime
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-event-series-schema.json
slug: argo-cd-v1-event-series
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-series-schema.json\",\n  \"title\": \"v1EventSeries\",\n  \"description\": \"EventSeries contain information on series of events, i.e. thing that was/is happening\\ncontinuously for some time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"title\": \"Number of occurrences in this series up to the last heartbeat time\"\n    },\n    \"lastObservedTime\": {\n      \"$ref\": \"#/definitions/v1MicroTime\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-series-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1EventSeries
---
