---
description: ClusterConfig is the configuration attributes. This structure is subset of the go-client rest.Config with annotations added for marshalling.
layout: schema
name: v1alpha1ClusterConfig
properties_list:
- description: ''
  name: awsAuthConfig
  type: object
- description: 'Server requires Bearer authentication. This client will not attempt to use refresh tokens for an OAuth2 flow. TODO: demonstrate an OAuth2 compatible client.'
  name: bearerToken
  type: string
- description: DisableCompression bypasses automatic GZip compression requests to the server.
  name: disableCompression
  type: boolean
- description: ''
  name: execProviderConfig
  type: object
- description: ''
  name: password
  type: string
- description: ''
  name: proxyUrl
  type: string
- description: ''
  name: tlsClientConfig
  type: object
- description: ''
  name: username
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-config-schema.json
slug: argo-cd-v1alpha1-cluster-config
source_filename: argo-cd-v1alpha1-cluster-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-config-schema.json\",\n  \"title\": \"v1alpha1ClusterConfig\",\n  \"description\": \"ClusterConfig is the configuration attributes. This structure is subset of the go-client\\nrest.Config with annotations added for marshalling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsAuthConfig\": {\n      \"$ref\": \"#/definitions/v1alpha1AWSAuthConfig\"\n    },\n    \"bearerToken\": {\n      \"description\": \"Server requires Bearer authentication. This client will not attempt to use\\nrefresh tokens for an OAuth2 flow.\\nTODO: demonstrate an OAuth2 compatible client.\",\n      \"type\": \"string\"\n    },\n    \"disableCompression\": {\n      \"description\": \"DisableCompression bypasses automatic GZip compression requests to the server.\",\n      \"type\": \"boolean\"\n    },\n\
  \    \"execProviderConfig\": {\n      \"$ref\": \"#/definitions/v1alpha1ExecProviderConfig\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"proxyUrl\": {\n      \"type\": \"string\",\n      \"title\": \"ProxyURL is the URL to the proxy to be used for all requests send to the server\"\n    },\n    \"tlsClientConfig\": {\n      \"$ref\": \"#/definitions/v1alpha1TLSClientConfig\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Server requires Basic authentication\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-config-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterConfig
---
