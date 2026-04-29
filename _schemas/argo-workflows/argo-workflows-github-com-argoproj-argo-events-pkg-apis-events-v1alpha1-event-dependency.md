---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependency schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependency
properties_list:
- description: ''
  name: eventName
  type: string
- description: ''
  name: eventSourceName
  type: string
- description: ''
  name: filters
  type: object
- description: 'FiltersLogicalOperator defines how different filters are evaluated together. Available values: and (&&), or (||) Is optional and if left blank treated as and (&&).'
  name: filtersLogicalOperator
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: transform
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependency\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependency schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventName\": {\n      \"type\": \"string\",\n      \"title\": \"EventName is the name of the event\"\n    },\n    \"eventSourceName\": {\n      \"type\": \"string\",\n      \"title\": \"EventSourceName is the name of EventSource that Sensor depends on\"\n    },\n    \"filters\": {\n      \"title\": \"Filters and rules governing toleration of success and constraints on the context and data of an event\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependencyFilter\"\
  \n    },\n    \"filtersLogicalOperator\": {\n      \"description\": \"FiltersLogicalOperator defines how different filters are evaluated together.\\nAvailable values: and (&&), or (||)\\nIs optional and if left blank treated as and (&&).\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name is a unique name of this dependency\"\n    },\n    \"transform\": {\n      \"title\": \"Transform transforms the event data\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependencyTransformer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependency
---
