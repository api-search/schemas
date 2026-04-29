---
description: clusterOIDCConfig schema from Argo CD API
layout: schema
name: clusterOIDCConfig
properties_list:
- description: ''
  name: cliClientID
  type: string
- description: ''
  name: clientID
  type: string
- description: ''
  name: enablePKCEAuthentication
  type: boolean
- description: ''
  name: idTokenClaims
  type: object
- description: ''
  name: issuer
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: scopes
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-oidc-config-schema.json
slug: argo-cd-cluster-oidc-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-oidc-config-schema.json\",\n  \"title\": \"clusterOIDCConfig\",\n  \"description\": \"clusterOIDCConfig schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cliClientID\": {\n      \"type\": \"string\"\n    },\n    \"clientID\": {\n      \"type\": \"string\"\n    },\n    \"enablePKCEAuthentication\": {\n      \"type\": \"boolean\"\n    },\n    \"idTokenClaims\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/oidcClaim\"\n      }\n    },\n    \"issuer\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-oidc-config-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterOIDCConfig
---
