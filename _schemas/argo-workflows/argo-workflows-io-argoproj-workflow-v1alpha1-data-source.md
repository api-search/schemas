---
description: DataSource sources external data into a data template
layout: schema
name: io.argoproj.workflow.v1alpha1.DataSource
properties_list:
- description: ArtifactPaths is a data transformation that collects a list of artifact paths
  name: artifactPaths
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-data-source-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-data-source
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-data-source-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.DataSource\",\n  \"description\": \"DataSource sources external data into a data template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifactPaths\": {\n      \"description\": \"ArtifactPaths is a data transformation that collects a list of artifact paths\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtifactPaths\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-data-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.DataSource
---
