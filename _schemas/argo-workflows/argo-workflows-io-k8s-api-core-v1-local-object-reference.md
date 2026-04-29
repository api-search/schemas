---
description: LocalObjectReference contains enough information to let you locate the referenced object inside the same namespace.
layout: schema
name: io.k8s.api.core.v1.LocalObjectReference
properties_list:
- description: Name of the referent. This field is effectively required, but due to backwards compatibility is allowed to be empty. Instances of this type with an empty value here are almost certainly wrong. More in
  name: name
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-local-object-reference-schema.json
slug: argo-workflows-io-k8s-api-core-v1-local-object-reference
source_filename: argo-workflows-io-k8s-api-core-v1-local-object-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-local-object-reference-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.LocalObjectReference\",\n  \"description\": \"LocalObjectReference contains enough information to let you locate the referenced object inside the same namespace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of the referent. This field is effectively required, but due to backwards compatibility is allowed to be empty. Instances of this type with an empty value here are almost certainly wrong. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-local-object-reference-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.LocalObjectReference
---
