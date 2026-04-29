---
description: SecretKeySelector selects a key of a Secret.
layout: schema
name: io.k8s.api.core.v1.SecretKeySelector
properties_list:
- description: The key of the secret to select from. Must be a valid secret key.
  name: key
  type: string
- description: Name of the referent. This field is effectively required, but due to backwards compatibility is allowed to be empty. Instances of this type with an empty value here are almost certainly wrong. More in
  name: name
  type: string
- description: Specify whether the Secret or its key must be defined
  name: optional
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-secret-key-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-secret-key-selector
source_filename: argo-workflows-io-k8s-api-core-v1-secret-key-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-secret-key-selector-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.SecretKeySelector\",\n  \"description\": \"SecretKeySelector selects a key of a Secret.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"The key of the secret to select from.  Must be a valid secret key.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the referent. This field is effectively required, but due to backwards compatibility is allowed to be empty. Instances of this type with an empty value here are almost certainly wrong. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names\",\n      \"type\": \"string\"\n    },\n    \"optional\": {\n      \"description\": \"Specify whether\
  \ the Secret or its key must be defined\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-secret-key-selector-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SecretKeySelector
---
