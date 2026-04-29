---
description: SCMProviderGeneratorBitbucketServer defines connection info specific to Bitbucket Server.
layout: schema
name: v1alpha1SCMProviderGeneratorBitbucketServer
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The Bitbucket Server REST API URL to talk to. Required.
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
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-server-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-bitbucket-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-server-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorBitbucketServer\",\n  \"description\": \"SCMProviderGeneratorBitbucketServer defines connection info specific to Bitbucket Server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the default branch.\",\n      \"type\": \"boolean\"\n    },\n    \"api\": {\n      \"description\": \"The Bitbucket Server REST API URL to talk to. Required.\",\n      \"type\": \"string\"\n    },\n    \"basicAuth\": {\n      \"$ref\": \"#/definitions/v1alpha1BasicAuthBitbucketServer\"\n    },\n    \"bearerToken\": {\n      \"$ref\": \"#/definitions/v1alpha1BearerTokenBitbucket\"\n    },\n    \"caRef\": {\n      \"$ref\": \"#/definitions/v1alpha1ConfigMapKeyRef\"\
  \n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Allow self-signed TLS / Certificates; default: false\"\n    },\n    \"project\": {\n      \"description\": \"Project to scan. Required.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-server-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorBitbucketServer
---
