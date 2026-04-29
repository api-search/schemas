---
description: v1alpha1TLSClientConfig schema from Argo CD API
layout: schema
name: v1alpha1TLSClientConfig
properties_list:
- description: ''
  name: caData
  type: string
- description: ''
  name: certData
  type: string
- description: Insecure specifies that the server should be accessed without verifying the TLS certificate. For testing only.
  name: insecure
  type: boolean
- description: ''
  name: keyData
  type: string
- description: ServerName is passed to the server for SNI and is used in the client to check server certificates against. If ServerName is empty, the hostname used to contact the server is used.
  name: serverName
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-tls-client-config-schema.json
slug: argo-cd-v1alpha1-tls-client-config
source_filename: argo-cd-v1alpha1-tls-client-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-tls-client-config-schema.json\",\n  \"title\": \"v1alpha1TLSClientConfig\",\n  \"description\": \"v1alpha1TLSClientConfig schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"caData\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"title\": \"CAData holds PEM-encoded bytes (typically read from a root certificates bundle).\\nCAData takes precedence over CAFile\"\n    },\n    \"certData\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"title\": \"CertData holds PEM-encoded bytes (typically read from a client certificate file).\\nCertData takes precedence over CertFile\"\n    },\n    \"insecure\": {\n      \"description\": \"Insecure specifies that the server should be accessed without verifying the TLS certificate. For testing\
  \ only.\",\n      \"type\": \"boolean\"\n    },\n    \"keyData\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"title\": \"KeyData holds PEM-encoded bytes (typically read from a client certificate key file).\\nKeyData takes precedence over KeyFile\"\n    },\n    \"serverName\": {\n      \"description\": \"ServerName is passed to the server for SNI and is used in the client to check server\\ncertificates against. If ServerName is empty, the hostname used to contact the\\nserver is used.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-tls-client-config-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1TLSClientConfig
---
