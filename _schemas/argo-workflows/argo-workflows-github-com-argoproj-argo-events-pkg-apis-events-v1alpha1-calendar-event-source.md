---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CalendarEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CalendarEventSource
properties_list:
- description: ExclusionDates defines the list of DATE-TIME exceptions for recurring events.
  name: exclusionDates
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: interval
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: persistence
  type: object
- description: ''
  name: schedule
  type: string
- description: ''
  name: timezone
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-calendar-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-calendar-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-calendar-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-calendar-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CalendarEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CalendarEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exclusionDates\": {\n      \"description\": \"ExclusionDates defines the list of DATE-TIME exceptions for recurring events.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"interval\": {\n\
  \      \"type\": \"string\",\n      \"title\": \"Interval is a string that describes an interval duration, e.g. 1s, 30m, 2h...\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"persistence\": {\n      \"title\": \"Persistence hold the configuration for event persistence\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventPersistence\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"title\": \"Schedule is a cron-like expression. For reference, see: https://en.wikipedia.org/wiki/Cron\\n+optional\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"title\": \"Timezone in which to run the schedule\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-calendar-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CalendarEventSource
---
