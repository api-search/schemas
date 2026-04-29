---
description: TimeFilter describes a window in time. It filters out events that occur outside the time limits. In other words, only events that occur after Start and before Stop will pass this filter.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TimeFilter
properties_list:
- description: Start is the beginning of a time window in UTC. Before this time, events for this dependency are ignored. Format is hh:mm:ss.
  name: start
  type: string
- description: Stop is the end of a time window in UTC. After or equal to this time, events for this dependency are ignored and Format is hh:mm:ss. If it is smaller than Start, it is treated as next day of Start (e.
  name: stop
  type: string
- description: ''
  name: timezone
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-time-filter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-time-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-time-filter-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TimeFilter\",\n  \"description\": \"TimeFilter describes a window in time.\\nIt filters out events that occur outside the time limits.\\nIn other words, only events that occur after Start and before Stop\\nwill pass this filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"description\": \"Start is the beginning of a time window in UTC.\\nBefore this time, events for this dependency are ignored.\\nFormat is hh:mm:ss.\",\n      \"type\": \"string\"\n    },\n    \"stop\": {\n      \"description\": \"Stop is the end of a time window in UTC.\\nAfter or equal to this time, events for this dependency are ignored\
  \ and\\nFormat is hh:mm:ss.\\nIf it is smaller than Start, it is treated as next day of Start\\n(e.g.: 22:00:00-01:00:00 means 22:00:00-25:00:00).\",\n      \"type\": \"string\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"title\": \"Timezone specifies the timezone for the time window.\\nIf not specified, defaults to UTC.\\nFormat should be a valid IANA timezone name (e.g., \\\"America/New_York\\\", \\\"Europe/London\\\").\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-time-filter-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TimeFilter
---
