---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact
properties_list:
- description: ''
  name: branch
  type: string
- description: Directory to clone the repository. We clone complete directory because GitArtifact is not limited to any specific Git service providers. Hence we don't use any specific git provider client.
  name: cloneDirectory
  type: string
- description: ''
  name: creds
  type: object
- description: ''
  name: filePath
  type: string
- description: ''
  name: insecureIgnoreHostKey
  type: boolean
- description: ''
  name: ref
  type: string
- description: ''
  name: remote
  type: object
- description: ''
  name: sshKeySecret
  type: object
- description: ''
  name: tag
  type: string
- description: ''
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-artifact-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-artifact-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"type\": \"string\",\n      \"title\": \"Branch to use to pull trigger resource\\n+optional\"\n    },\n    \"cloneDirectory\": {\n      \"description\": \"Directory to clone the repository. We clone complete directory because GitArtifact is not limited to any specific Git service providers.\\nHence we don't use any specific git provider client.\",\n      \"type\": \"string\"\n    },\n    \"creds\": {\n      \"title\": \"Creds\
  \ contain reference to git username and password\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitCreds\"\n    },\n    \"filePath\": {\n      \"type\": \"string\",\n      \"title\": \"Path to file that contains trigger resource definition\"\n    },\n    \"insecureIgnoreHostKey\": {\n      \"type\": \"boolean\",\n      \"title\": \"Whether to ignore host key\\n+optional\"\n    },\n    \"ref\": {\n      \"type\": \"string\",\n      \"title\": \"Ref to use to pull trigger resource. Will result in a shallow clone and\\nfetch.\\n+optional\"\n    },\n    \"remote\": {\n      \"title\": \"Remote to manage set of tracked repositories. Defaults to \\\"origin\\\".\\nRefer https://git-scm.com/docs/git-remote\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitRemoteConfig\"\n    },\n    \"sshKeySecret\": {\n      \"title\": \"SSHKeySecret refers to the secret that contains SSH key\"\
  ,\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"title\": \"Tag to use to pull trigger resource\\n+optional\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"title\": \"Git URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact
---
