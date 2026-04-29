---
description: SFTPEventSource describes an event-source for sftp related events.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SFTPEventSource
properties_list:
- description: Address sftp address.
  name: address
  type: object
- description: ''
  name: eventType
  type: string
- description: ''
  name: filter
  type: object
- description: ''
  name: metadata
  type: object
- description: Password required for authentication if any.
  name: password
  type: object
- description: ''
  name: pollIntervalDuration
  type: string
- description: SSHKeySecret refers to the secret that contains SSH key. Key needs to contain private key and public key.
  name: sshKeySecret
  type: object
- description: Username required for authentication if any.
  name: username
  type: object
- description: ''
  name: watchPathConfig
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SFTPEventSource\",\n  \"description\": \"SFTPEventSource describes an event-source for sftp related events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"Address sftp address.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"title\": \"Type of file operations to watch\\nRefer https://github.com/fsnotify/fsnotify/blob/master/fsnotify.go for more information\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\
  \n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"password\": {\n      \"description\": \"Password required for authentication if any.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"pollIntervalDuration\": {\n      \"type\": \"string\",\n      \"title\": \"PollIntervalDuration the interval at which to poll the SFTP server\\ndefaults to 10 seconds\\n+optional\"\n    },\n    \"sshKeySecret\": {\n      \"description\": \"SSHKeySecret refers to the secret that contains SSH key. Key needs to contain private key and public key.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"username\": {\n      \"description\": \"Username required for authentication if any.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\
  \n    },\n    \"watchPathConfig\": {\n      \"title\": \"WatchPathConfig contains configuration about the file path to watch\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WatchPathConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SFTPEventSource
---
