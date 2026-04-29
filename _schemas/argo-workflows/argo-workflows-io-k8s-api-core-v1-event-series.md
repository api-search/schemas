---
description: EventSeries contain information on series of events, i.e. thing that was/is happening continuously for some time.
layout: schema
name: io.k8s.api.core.v1.EventSeries
properties_list:
- description: Number of occurrences in this series up to the last heartbeat time
  name: count
  type: integer
- description: Time of the last occurrence observed
  name: lastObservedTime
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-event-series-schema.json
slug: argo-workflows-io-k8s-api-core-v1-event-series
source_filename: argo-workflows-io-k8s-api-core-v1-event-series-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-event-series-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EventSeries\",\n  \"description\": \"EventSeries contain information on series of events, i.e. thing that was/is happening continuously for some time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"description\": \"Number of occurrences in this series up to the last heartbeat time\",\n      \"type\": \"integer\"\n    },\n    \"lastObservedTime\": {\n      \"description\": \"Time of the last occurrence observed\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.MicroTime\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-event-series-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EventSeries
---
