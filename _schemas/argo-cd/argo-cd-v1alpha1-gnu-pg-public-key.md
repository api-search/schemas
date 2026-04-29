---
description: v1alpha1GnuPGPublicKey schema from Argo CD API
layout: schema
name: v1alpha1GnuPGPublicKey
properties_list:
- description: ''
  name: fingerprint
  type: string
- description: ''
  name: keyData
  type: string
- description: ''
  name: keyID
  type: string
- description: ''
  name: owner
  type: string
- description: ''
  name: subType
  type: string
- description: ''
  name: trust
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-gnu-pg-public-key-schema.json
slug: argo-cd-v1alpha1-gnu-pg-public-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-gnu-pg-public-key-schema.json\",\n  \"title\": \"v1alpha1GnuPGPublicKey\",\n  \"description\": \"v1alpha1GnuPGPublicKey schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"title\": \"Fingerprint is the fingerprint of the key\"\n    },\n    \"keyData\": {\n      \"type\": \"string\",\n      \"title\": \"KeyData holds the raw key data, in base64 encoded format\"\n    },\n    \"keyID\": {\n      \"type\": \"string\",\n      \"title\": \"KeyID specifies the key ID, in hexadecimal string format\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"title\": \"Owner holds the owner identification, e.g. a name and e-mail address\"\n    },\n    \"subType\": {\n      \"type\": \"string\",\n      \"title\": \"\
  SubType holds the key's subtype (e.g. rsa4096)\"\n    },\n    \"trust\": {\n      \"type\": \"string\",\n      \"title\": \"Trust holds the level of trust assigned to this key\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-gnu-pg-public-key-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1GnuPGPublicKey
---
