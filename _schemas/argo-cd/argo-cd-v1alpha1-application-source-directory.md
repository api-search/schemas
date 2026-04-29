---
description: v1alpha1ApplicationSourceDirectory schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourceDirectory
properties_list:
- description: ''
  name: exclude
  type: string
- description: ''
  name: include
  type: string
- description: ''
  name: jsonnet
  type: object
- description: ''
  name: recurse
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-directory-schema.json
slug: argo-cd-v1alpha1-application-source-directory
source_filename: argo-cd-v1alpha1-application-source-directory-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-directory-schema.json\",\n  \"title\": \"v1alpha1ApplicationSourceDirectory\",\n  \"description\": \"v1alpha1ApplicationSourceDirectory schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exclude\": {\n      \"type\": \"string\",\n      \"title\": \"Exclude contains a glob pattern to match paths against that should be explicitly excluded from being used during manifest generation\"\n    },\n    \"include\": {\n      \"type\": \"string\",\n      \"title\": \"Include contains a glob pattern to match paths against that should be explicitly included during manifest generation\"\n    },\n    \"jsonnet\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceJsonnet\"\n    },\n    \"recurse\": {\n      \"type\": \"boolean\",\n      \"title\": \"Recurse\
  \ specifies whether to scan a directory recursively for manifests\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-directory-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourceDirectory
---
