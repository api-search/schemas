---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource
properties_list:
- description: ''
  name: accessToken
  type: object
- description: BitbucketServerBaseURL is the base URL for API requests to a custom endpoint.
  name: bitbucketserverBaseURL
  type: string
- description: ''
  name: checkInterval
  type: string
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
  name: metadata
  type: object
- description: ''
  name: oneEventPerChange
  type: boolean
- description: ''
  name: projectKey
  type: string
- description: ''
  name: projects
  type: array
- description: ''
  name: repositories
  type: array
- description: ''
  name: repositorySlug
  type: string
- description: ''
  name: skipBranchRefsChangedOnOpenPR
  type: boolean
- description: ''
  name: tls
  type: object
- description: Webhook holds configuration to run a http server.
  name: webhook
  type: object
- description: ''
  name: webhookSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessToken\": {\n      \"title\": \"AccessToken is reference to K8s secret which holds the bitbucket api access information.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"bitbucketserverBaseURL\": {\n      \"description\": \"BitbucketServerBaseURL is the base URL for API requests to a custom endpoint.\",\n      \"type\": \"string\"\n    },\n\
  \    \"checkInterval\": {\n      \"type\": \"string\",\n      \"title\": \"CheckInterval is a duration in which to wait before checking that the webhooks exist, e.g. 1s, 30m, 2h... (defaults to 1m)\\n+optional\"\n    },\n    \"deleteHookOnFinish\": {\n      \"type\": \"boolean\",\n      \"title\": \"DeleteHookOnFinish determines whether to delete the Bitbucket Server hook for the project once the event source is stopped.\\n+optional\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"title\": \"Events are bitbucket event to listen to.\\nRefer https://confluence.atlassian.com/bitbucketserver/event-payload-938025882.html\\n+optional\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined\
  \ metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"oneEventPerChange\": {\n      \"type\": \"boolean\",\n      \"title\": \"OneEventPerChange controls whether to process each change in a repo:refs_changed webhook event as a separate io.argoproj.workflow.v1alpha1. This setting is useful when multiple tags are\\npushed simultaneously for the same commit, and each tag needs to independently trigger an action, such as a distinct workflow in Argo Workflows. When enabled, the\\nBitbucketServerEventSource publishes an individual BitbucketServerEventData for each change, ensuring independent processing of each tag or reference update in a\\nsingle webhook event.\\n+optional\"\n    },\n    \"projectKey\": {\n      \"type\": \"string\",\n      \"title\": \"DeprecatedProjectKey is the key of project for which integration needs to set up.\\nDeprecated: use Repositories instead. Will be unsupported\
  \ in v1.8.\\n+optional\"\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"title\": \"Projects holds a list of projects for which integration needs to set up, this will add the webhook to all repositories in the project.\\n+optional\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"repositories\": {\n      \"type\": \"array\",\n      \"title\": \"Repositories holds a list of repositories for which integration needs to set up.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerRepository\"\n      }\n    },\n    \"repositorySlug\": {\n      \"type\": \"string\",\n      \"title\": \"DeprecatedRepositorySlug is the slug of the repository for which integration needs to set up.\\nDeprecated: use Repositories instead. Will be unsupported in v1.8.\\n+optional\"\n    },\n    \"skipBranchRefsChangedOnOpenPR\": {\n      \"type\": \"boolean\",\n      \"title\": \"SkipBranchRefsChangedOnOpenPR\
  \ bypasses the event repo:refs_changed for branches whenever there's an associated open pull request.\\nThis helps in optimizing the event handling process by avoiding unnecessary triggers for branch reference changes that are already part of a pull request under review.\\n+optional\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the bitbucketserver client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"webhook\": {\n      \"description\": \"Webhook holds configuration to run a http server.\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\n    },\n    \"webhookSecret\": {\n      \"title\": \"WebhookSecret is reference to K8s secret which holds the bitbucket webhook secret (for HMAC validation).\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource
---
