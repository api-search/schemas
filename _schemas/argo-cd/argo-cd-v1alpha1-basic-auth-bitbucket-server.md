---
description: BasicAuthBitbucketServer defines the username/(password or personal access token) for Basic auth.
layout: schema
name: v1alpha1BasicAuthBitbucketServer
properties_list:
- description: ''
  name: passwordRef
  type: object
- description: ''
  name: username
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-basic-auth-bitbucket-server-schema.json
slug: argo-cd-v1alpha1-basic-auth-bitbucket-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-basic-auth-bitbucket-server-schema.json\",\n  \"title\": \"v1alpha1BasicAuthBitbucketServer\",\n  \"description\": \"BasicAuthBitbucketServer defines the username/(password or personal access token) for Basic auth.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"passwordRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username for Basic auth\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-basic-auth-bitbucket-server-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1BasicAuthBitbucketServer
---
