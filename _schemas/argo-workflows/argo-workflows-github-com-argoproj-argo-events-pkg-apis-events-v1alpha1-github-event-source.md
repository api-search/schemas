---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource
properties_list:
- description: ''
  name: active
  type: boolean
- description: ''
  name: apiToken
  type: object
- description: ''
  name: contentType
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
  name: githubApp
  type: object
- description: ''
  name: githubBaseURL
  type: string
- description: ''
  name: githubUploadURL
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: metadata
  type: object
- description: Organizations holds the names of organizations (used for organization level webhooks). Not required if Repositories is set.
  name: organizations
  type: array
- description: ''
  name: owner
  type: string
- description: Repositories holds the information of repositories, which uses repo owner as the key, and list of repo names as the value. Not required if Organizations is set.
  name: repositories
  type: array
- description: ''
  name: repository
  type: string
- description: ''
  name: webhook
  type: object
- description: ''
  name: webhookSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"type\": \"boolean\",\n      \"title\": \"Active refers to status of the webhook for event deliveries.\\nhttps://developer.github.com/webhooks/creating/#active\\n+optional\"\n    },\n    \"apiToken\": {\n      \"title\": \"APIToken refers to a K8s secret containing github api token\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"contentType\": {\n     \
  \ \"type\": \"string\",\n      \"title\": \"ContentType of the event delivery\"\n    },\n    \"deleteHookOnFinish\": {\n      \"type\": \"boolean\",\n      \"title\": \"DeleteHookOnFinish determines whether to delete the GitHub hook for the repository once the event source is stopped.\\n+optional\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"title\": \"Events refer to Github events to which the event source will subscribe\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"githubApp\": {\n      \"title\": \"GitHubApp holds the GitHub app credentials\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubAppCreds\"\n    },\n    \"githubBaseURL\": {\n      \"type\": \"string\",\n      \"title\": \"GitHub base URL\
  \ (for GitHub Enterprise)\\n+optional\"\n    },\n    \"githubUploadURL\": {\n      \"type\": \"string\",\n      \"title\": \"GitHub upload URL (for GitHub Enterprise)\\n+optional\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"title\": \"Id is the webhook's id\\nDeprecated: This is not used at all, will be removed in v1.6\\n+optional\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Insecure tls verification\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"organizations\": {\n      \"description\": \"Organizations holds the names of organizations (used for organization level webhooks). Not required if Repositories is set.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"\
  owner\": {\n      \"type\": \"string\",\n      \"title\": \"DeprecatedOwner refers to GitHub owner name i.e. argoproj\\nDeprecated: use Repositories instead. Will be unsupported in v 1.6\\n+optional\"\n    },\n    \"repositories\": {\n      \"description\": \"Repositories holds the information of repositories, which uses repo owner as the key,\\nand list of repo names as the value. Not required if Organizations is set.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OwnedRepositories\"\n      }\n    },\n    \"repository\": {\n      \"type\": \"string\",\n      \"title\": \"DeprecatedRepository refers to GitHub repo name i.e. argo-events\\nDeprecated: use Repositories instead. Will be unsupported in v 1.6\\n+optional\"\n    },\n    \"webhook\": {\n      \"title\": \"Webhook refers to the configuration required to run a http server\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\
  \n    },\n    \"webhookSecret\": {\n      \"title\": \"WebhookSecret refers to K8s secret containing GitHub webhook secret\\nhttps://developer.github.com/webhooks/securing/\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource
---
