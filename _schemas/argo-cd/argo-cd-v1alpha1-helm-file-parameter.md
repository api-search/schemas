---
description: v1alpha1HelmFileParameter schema from Argo CD API
layout: schema
name: v1alpha1HelmFileParameter
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: path
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-helm-file-parameter-schema.json
slug: argo-cd-v1alpha1-helm-file-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-helm-file-parameter-schema.json\",\n  \"title\": \"v1alpha1HelmFileParameter\",\n  \"description\": \"v1alpha1HelmFileParameter schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name is the name of the Helm parameter\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"title\": \"Path is the path to the file containing the values for the Helm parameter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-helm-file-parameter-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HelmFileParameter
---
