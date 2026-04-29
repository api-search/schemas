---
description: gpgkeyGnuPGPublicKeyCreateResponse schema from Argo CD API
layout: schema
name: gpgkeyGnuPGPublicKeyCreateResponse
properties_list:
- description: ''
  name: created
  type: object
- description: ''
  name: skipped
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-gpgkey-gnu-pg-public-key-create-response-schema.json
slug: argo-cd-gpgkey-gnu-pg-public-key-create-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-gpgkey-gnu-pg-public-key-create-response-schema.json\",\n  \"title\": \"gpgkeyGnuPGPublicKeyCreateResponse\",\n  \"description\": \"gpgkeyGnuPGPublicKeyCreateResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created\": {\n      \"$ref\": \"#/definitions/v1alpha1GnuPGPublicKeyList\"\n    },\n    \"skipped\": {\n      \"type\": \"array\",\n      \"title\": \"List of key IDs that haven been skipped because they already exist on the server\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-gpgkey-gnu-pg-public-key-create-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: gpgkeyGnuPGPublicKeyCreateResponse
---
