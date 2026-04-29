---
description: ArchiveStrategy describes how to archive files/directory when saving artifacts
layout: schema
name: io.argoproj.workflow.v1alpha1.ArchiveStrategy
properties_list:
- description: ''
  name: none
  type: object
- description: ''
  name: tar
  type: object
- description: ''
  name: zip
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-archive-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-archive-strategy
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-archive-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-archive-strategy-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArchiveStrategy\",\n  \"description\": \"ArchiveStrategy describes how to archive files/directory when saving artifacts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"none\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.NoneStrategy\"\n    },\n    \"tar\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.TarStrategy\"\n    },\n    \"zip\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ZipStrategy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-archive-strategy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArchiveStrategy
---
