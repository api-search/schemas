---
description: BearerTokenBitbucketCloud defines the Bearer token for BitBucket AppToken auth.
layout: schema
name: v1alpha1BearerTokenBitbucketCloud
properties_list:
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-bearer-token-bitbucket-cloud-schema.json
slug: argo-cd-v1alpha1-bearer-token-bitbucket-cloud
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-bearer-token-bitbucket-cloud-schema.json\",\n  \"title\": \"v1alpha1BearerTokenBitbucketCloud\",\n  \"description\": \"BearerTokenBitbucketCloud defines the Bearer token for BitBucket AppToken auth.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-bearer-token-bitbucket-cloud-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1BearerTokenBitbucketCloud
---
