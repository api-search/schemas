---
description: Memoize enables caching for the Outputs of the template.
layout: schema
name: io.argoproj.workflow.v1alpha1.Memoize
properties_list:
- description: Cache sets and configures the kind of cache
  name: cache
  type: object
- description: Key is the key to use as the caching key
  name: key
  type: string
- description: MaxAge is the maximum age (e.g. "180s", "24h") of an entry that is still considered valid. If an entry is older than the MaxAge, it will be ignored.
  name: maxAge
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoize-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-memoize
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-memoize-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoize-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Memoize\",\n  \"description\": \"Memoize enables caching for the Outputs of the template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cache\": {\n      \"description\": \"Cache sets and configures the kind of cache\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Cache\"\n    },\n    \"key\": {\n      \"description\": \"Key is the key to use as the caching key\",\n      \"type\": \"string\"\n    },\n    \"maxAge\": {\n      \"description\": \"MaxAge is the maximum age (e.g. \\\"180s\\\", \\\"24h\\\") of an entry that is still considered valid. If an entry is older than the MaxAge, it will be ignored.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n\
  \    \"key\",\n    \"cache\",\n    \"maxAge\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoize-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Memoize
---
