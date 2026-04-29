---
description: Status of the build execution.
layout: schema
name: BuildStatus
properties_list:
- description: The current phase of the build.
  name: phase
  type: string
- description: Whether the build was cancelled.
  name: cancelled
  type: boolean
- description: Human-readable message about the build status.
  name: message
  type: string
- description: Brief machine-readable reason for the build status.
  name: reason
  type: string
- description: Timestamp when the build started running.
  name: startTimestamp
  type: string
- description: Timestamp when the build completed.
  name: completionTimestamp
  type: string
- description: Duration of the build in nanoseconds.
  name: duration
  type: integer
- description: The Docker image reference of the built image.
  name: outputDockerImageReference
  type: string
- description: Build output details.
  name: output
  type: object
- description: The last few lines of the build log for failed builds.
  name: logSnippet
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-status-schema.json
slug: openshift-rest-build-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of the build execution.\",\n  \"properties\": {\n    \"phase\": {\n      \"type\": \"string\",\n      \"description\": \"The current phase of the build.\"\n    },\n    \"cancelled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the build was cancelled.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable message about the build status.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Brief machine-readable reason for the build status.\"\n    },\n    \"startTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the build started running.\"\n    },\n    \"completionTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the build completed.\"\n    },\n    \"duration\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Duration of the build in nanoseconds.\"\n    },\n    \"outputDockerImageReference\": {\n      \"type\": \"string\",\n      \"description\": \"The Docker image reference of the built image.\"\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Build output details.\"\n    },\n    \"logSnippet\": {\n      \"type\": \"string\",\n      \"description\": \"The last few lines of the build log for failed builds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-status-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildStatus
---
