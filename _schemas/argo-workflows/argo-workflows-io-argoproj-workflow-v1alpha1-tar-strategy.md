---
description: TarStrategy will tar and gzip the file or directory when saving
layout: schema
name: io.argoproj.workflow.v1alpha1.TarStrategy
properties_list:
- description: CompressionLevel specifies the gzip compression level to use for the artifact. Defaults to gzip.DefaultCompression.
  name: compressionLevel
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-tar-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-tar-strategy
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-tar-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-tar-strategy-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.TarStrategy\",\n  \"description\": \"TarStrategy will tar and gzip the file or directory when saving\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"compressionLevel\": {\n      \"description\": \"CompressionLevel specifies the gzip compression level to use for the artifact. Defaults to gzip.DefaultCompression.\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-tar-strategy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.TarStrategy
---
