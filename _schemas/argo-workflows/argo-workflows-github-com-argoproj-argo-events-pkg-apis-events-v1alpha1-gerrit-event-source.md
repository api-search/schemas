---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GerritEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GerritEventSource
properties_list:
- description: ''
  name: auth
  type: object
- description: ''
  name: deleteHookOnFinish
  type: boolean
- description: ''
  name: events
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: gerritBaseURL
  type: string
- description: ''
  name: hookName
  type: string
- description: ''
  name: maxTries
  type: string
- description: ''
  name: metadata
  type: object
- description: List of project namespace paths like "whynowy/test".
  name: projects
  type: array
- description: ''
  name: sslVerify
  type: boolean
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gerrit-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gerrit-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gerrit-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gerrit-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GerritEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GerritEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth\": {\n      \"title\": \"Auth hosts secret selectors for username and password\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth\"\n    },\n    \"deleteHookOnFinish\": {\n      \"type\": \"boolean\",\n      \"title\": \"DeleteHookOnFinish determines whether to delete the Gerrit hook for the project once the event source is stopped.\\n+optional\"\n    },\n \
  \   \"events\": {\n      \"type\": \"array\",\n      \"title\": \"Events are gerrit event to listen to.\\nRefer https://gerrit-review.googlesource.com/Documentation/cmd-stream-events.html#events\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"gerritBaseURL\": {\n      \"type\": \"string\",\n      \"title\": \"GerritBaseURL is the base URL for API requests to a custom endpoint\"\n    },\n    \"hookName\": {\n      \"type\": \"string\",\n      \"title\": \"HookName is the name of the webhook\"\n    },\n    \"maxTries\": {\n      \"type\": \"string\",\n      \"title\": \"MaxTries is number of attempts when posting an event to the target url\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed\
  \ along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"projects\": {\n      \"description\": \"List of project namespace paths like \\\"whynowy/test\\\".\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sslVerify\": {\n      \"type\": \"boolean\",\n      \"title\": \"SslVerify to enable ssl verification\\n+optional\"\n    },\n    \"webhook\": {\n      \"title\": \"Webhook holds configuration to run a http server\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gerrit-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GerritEventSource
---
