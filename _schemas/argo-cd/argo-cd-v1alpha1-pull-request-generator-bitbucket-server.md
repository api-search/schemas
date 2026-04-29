---
description: PullRequestGeneratorBitbucketServer defines connection info specific to BitbucketServer.
layout: schema
name: v1alpha1PullRequestGeneratorBitbucketServer
properties_list:
- description: The Bitbucket REST API URL to talk to e.g. https://bitbucket.org/rest Required.
  name: api
  type: string
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: bearerToken
  type: object
- description: ''
  name: caRef
  type: object
- description: ''
  name: insecure
  type: boolean
- description: Project to scan. Required.
  name: project
  type: string
- description: Repo name to scan. Required.
  name: repo
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-server-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-bitbucket-server
source_filename: argo-cd-v1alpha1-pull-request-generator-bitbucket-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-server-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorBitbucketServer\",\n  \"description\": \"PullRequestGeneratorBitbucketServer defines connection info specific to BitbucketServer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"description\": \"The Bitbucket REST API URL to talk to e.g. https://bitbucket.org/rest Required.\",\n      \"type\": \"string\"\n    },\n    \"basicAuth\": {\n      \"$ref\": \"#/definitions/v1alpha1BasicAuthBitbucketServer\"\n    },\n    \"bearerToken\": {\n      \"$ref\": \"#/definitions/v1alpha1BearerTokenBitbucket\"\n    },\n    \"caRef\": {\n      \"$ref\": \"#/definitions/v1alpha1ConfigMapKeyRef\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Allow self-signed\
  \ TLS / Certificates; default: false\"\n    },\n    \"project\": {\n      \"description\": \"Project to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"repo\": {\n      \"description\": \"Repo name to scan. Required.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-server-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorBitbucketServer
---
