---
description: SlackTrigger refers to the specification of the slack notification trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackTrigger
properties_list:
- description: ''
  name: attachments
  type: string
- description: ''
  name: blocks
  type: string
- description: ''
  name: channel
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: sender
  type: object
- description: SlackToken refers to the Kubernetes secret that holds the slack token required to send messages.
  name: slackToken
  type: object
- description: ''
  name: thread
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-slack-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-slack-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-slack-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackTrigger\",\n  \"description\": \"SlackTrigger refers to the specification of the slack notification trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attachments\": {\n      \"type\": \"string\",\n      \"title\": \"Attachments is a JSON format string that represents an array of Slack attachments according to the attachments API: https://api.slack.com/reference/messaging/attachments .\\n+optional\"\n    },\n    \"blocks\": {\n      \"type\": \"string\",\n      \"title\": \"Blocks is a JSON format string that represents an array of Slack blocks according to the blocks API: https://api.slack.com/reference/block-kit/blocks\
  \ .\\n+optional\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"title\": \"Channel refers to which Slack channel to send Slack message.\\n+optional\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message refers to the message to send to the Slack channel.\\n+optional\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is the list of key-value extracted from event's payload that are applied to\\nthe trigger resource.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"sender\": {\n      \"title\": \"Sender refers to additional configuration of the Slack application that sends the message.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackSender\"\n    },\n    \"slackToken\": {\n      \"description\": \"SlackToken refers to\
  \ the Kubernetes secret that holds the slack token required to send messages.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"thread\": {\n      \"title\": \"Thread refers to additional options for sending messages to a Slack thread.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackThread\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-slack-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackTrigger
---
