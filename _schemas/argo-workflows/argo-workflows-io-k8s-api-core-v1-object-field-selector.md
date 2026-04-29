---
description: ObjectFieldSelector selects an APIVersioned field of an object.
layout: schema
name: io.k8s.api.core.v1.ObjectFieldSelector
properties_list:
- description: Version of the schema the FieldPath is written in terms of, defaults to "v1".
  name: apiVersion
  type: string
- description: Path of the field to select in the specified API version.
  name: fieldPath
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-object-field-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-object-field-selector
source_filename: argo-workflows-io-k8s-api-core-v1-object-field-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-object-field-selector-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ObjectFieldSelector\",\n  \"description\": \"ObjectFieldSelector selects an APIVersioned field of an object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"Version of the schema the FieldPath is written in terms of, defaults to \\\"v1\\\".\",\n      \"type\": \"string\"\n    },\n    \"fieldPath\": {\n      \"description\": \"Path of the field to select in the specified API version.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"fieldPath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-object-field-selector-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ObjectFieldSelector
---
