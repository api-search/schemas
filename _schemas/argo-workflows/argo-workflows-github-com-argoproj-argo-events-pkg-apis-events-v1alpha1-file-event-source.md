---
description: FileEventSource describes an event-source for file related events.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.FileEventSource
properties_list:
- description: ''
  name: eventType
  type: string
- description: ''
  name: filter
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: polling
  type: boolean
- description: ''
  name: watchPathConfig
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-file-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-file-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-file-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.FileEventSource\",\n  \"description\": \"FileEventSource describes an event-source for file related events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"title\": \"Type of file operations to watch\\nRefer https://github.com/fsnotify/fsnotify/blob/master/fsnotify.go for more information\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined\
  \ metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"polling\": {\n      \"type\": \"boolean\",\n      \"title\": \"Use polling instead of inotify\"\n    },\n    \"watchPathConfig\": {\n      \"title\": \"WatchPathConfig contains configuration about the file path to watch\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WatchPathConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-file-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.FileEventSource
---
