---
description: v1alpha1KustomizeOptions schema from Argo CD API
layout: schema
name: v1alpha1KustomizeOptions
properties_list:
- description: 'Deprecated: Use settings.Settings instead. See: settings.Settings.KustomizeVersions. If this field is set, it will be used as the Kustomize binary path. Otherwise, Versions is used.'
  name: binaryPath
  type: string
- description: ''
  name: buildOptions
  type: string
- description: Versions is a list of Kustomize versions and their corresponding binary paths and build options.
  name: versions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-options-schema.json
slug: argo-cd-v1alpha1-kustomize-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-options-schema.json\",\n  \"title\": \"v1alpha1KustomizeOptions\",\n  \"description\": \"v1alpha1KustomizeOptions schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"binaryPath\": {\n      \"description\": \"Deprecated: Use settings.Settings instead. See: settings.Settings.KustomizeVersions.\\nIf this field is set, it will be used as the Kustomize binary path.\\nOtherwise, Versions is used.\",\n      \"type\": \"string\",\n      \"title\": \"BinaryPath holds optional path to kustomize binary\"\n    },\n    \"buildOptions\": {\n      \"type\": \"string\",\n      \"title\": \"BuildOptions is a string of build parameters to use when calling `kustomize build`\"\n    },\n    \"versions\": {\n      \"description\": \"Versions is a list of Kustomize versions and\
  \ their corresponding binary paths and build options.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1KustomizeVersion\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-options-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizeOptions
---
