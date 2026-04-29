---
description: PullRequestGeneratorBitbucket defines connection info specific to Bitbucket.
layout: schema
name: v1alpha1PullRequestGeneratorBitbucket
properties_list:
- description: The Bitbucket REST API URL to talk to. If blank, uses https://api.bitbucket.org/2.0.
  name: api
  type: string
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: bearerToken
  type: object
- description: Workspace to scan. Required.
  name: owner
  type: string
- description: Repo name to scan. Required.
  name: repo
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-bitbucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorBitbucket\",\n  \"description\": \"PullRequestGeneratorBitbucket defines connection info specific to Bitbucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"description\": \"The Bitbucket REST API URL to talk to. If blank, uses https://api.bitbucket.org/2.0.\",\n      \"type\": \"string\"\n    },\n    \"basicAuth\": {\n      \"$ref\": \"#/definitions/v1alpha1BasicAuthBitbucketServer\"\n    },\n    \"bearerToken\": {\n      \"$ref\": \"#/definitions/v1alpha1BearerTokenBitbucketCloud\"\n    },\n    \"owner\": {\n      \"description\": \"Workspace to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"repo\": {\n      \"description\": \"Repo name to scan. Required.\"\
  ,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorBitbucket
---
