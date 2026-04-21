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
