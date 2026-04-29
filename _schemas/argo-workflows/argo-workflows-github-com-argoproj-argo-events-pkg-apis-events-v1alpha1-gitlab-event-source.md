---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource
properties_list:
- description: ''
  name: accessToken
  type: object
- description: ''
  name: deleteHookOnFinish
  type: boolean
- description: ''
  name: enableSSLVerification
  type: boolean
- description: Events are gitlab event to listen to. Refer https://github.com/xanzy/go-gitlab/blob/bf34eca5d13a9f4c3f501d8a97b8ac226d55e4d9/projects.go#L794.
  name: events
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: gitlabBaseURL
  type: string
- description: ''
  name: groups
  type: array
- description: ''
  name: metadata
  type: object
- description: ''
  name: projectID
  type: string
- description: ''
  name: projects
  type: array
- description: ''
  name: secretToken
  type: object
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gitlab-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gitlab-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gitlab-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessToken\": {\n      \"title\": \"AccessToken references to k8 secret which holds the gitlab api access information\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"deleteHookOnFinish\": {\n      \"type\": \"boolean\",\n      \"title\": \"DeleteHookOnFinish determines whether to delete the GitLab hook for the project once the event source is stopped.\\n+optional\"\n    },\n    \"enableSSLVerification\"\
  : {\n      \"type\": \"boolean\",\n      \"title\": \"EnableSSLVerification to enable ssl verification\\n+optional\"\n    },\n    \"events\": {\n      \"description\": \"Events are gitlab event to listen to.\\nRefer https://github.com/xanzy/go-gitlab/blob/bf34eca5d13a9f4c3f501d8a97b8ac226d55e4d9/projects.go#L794.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"gitlabBaseURL\": {\n      \"type\": \"string\",\n      \"title\": \"GitlabBaseURL is the base URL for API requests to a custom endpoint\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"title\": \"List of group IDs or group name like \\\"test\\\".\\nGroup level hook available in Premium and Ultimate Gitlab.\\n+optional\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n\
  \    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"projectID\": {\n      \"type\": \"string\",\n      \"title\": \"DeprecatedProjectID is the id of project for which integration needs to setup\\nDeprecated: use Projects instead. Will be unsupported in v 1.7\\n+optional\"\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"title\": \"List of project IDs or project namespace paths like \\\"whynowy/test\\\".\\nIf neither a project nor a group is defined, the EventSource will not manage webhooks.\\n+optional\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"secretToken\": {\n      \"title\": \"SecretToken references to k8 secret which holds the Secret Token used by webhook config\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\
  \n    },\n    \"webhook\": {\n      \"title\": \"Webhook holds configuration to run a http server\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gitlab-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource
---
