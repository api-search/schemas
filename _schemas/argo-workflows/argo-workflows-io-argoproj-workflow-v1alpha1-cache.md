---
description: Cache is the configuration for the type of cache to be used
layout: schema
name: io.argoproj.workflow.v1alpha1.Cache
properties_list:
- description: ConfigMap sets a ConfigMap-based cache
  name: configMap
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cache-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-cache
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-cache-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cache-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Cache\",\n  \"description\": \"Cache is the configuration for the type of cache to be used\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMap\": {\n      \"description\": \"ConfigMap sets a ConfigMap-based cache\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n    }\n  },\n  \"required\": [\n    \"configMap\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cache-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Cache
---
