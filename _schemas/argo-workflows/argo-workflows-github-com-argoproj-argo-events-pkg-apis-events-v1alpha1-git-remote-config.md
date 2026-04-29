---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitRemoteConfig schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitRemoteConfig
properties_list:
- description: Name of the remote to fetch from.
  name: name
  type: string
- description: URLs the URLs of a remote repository. It must be non-empty. Fetch will always use the first URL, while push will use all of them.
  name: urls
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-remote-config-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-remote-config
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-remote-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-remote-config-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitRemoteConfig\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitRemoteConfig schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of the remote to fetch from.\",\n      \"type\": \"string\"\n    },\n    \"urls\": {\n      \"description\": \"URLs the URLs of a remote repository. It must be non-empty. Fetch will\\nalways use the first URL, while push will use all of them.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-remote-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitRemoteConfig
---
