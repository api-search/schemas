---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketAuth schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketAuth
properties_list:
- description: ''
  name: basic
  type: object
- description: ''
  name: oauthToken
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-auth-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-auth
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-auth-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketAuth\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketAuth schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basic\": {\n      \"title\": \"Basic is BasicAuth auth strategy.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketBasicAuth\"\n    },\n    \"oauthToken\": {\n      \"title\": \"OAuthToken refers to the K8s secret that holds the OAuth Bearer token.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-auth-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketAuth
---
