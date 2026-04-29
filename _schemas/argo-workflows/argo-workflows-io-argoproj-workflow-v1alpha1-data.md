---
description: Data is a data template
layout: schema
name: io.argoproj.workflow.v1alpha1.Data
properties_list:
- description: Source sources external data into a data template
  name: source
  type: object
- description: Transformation applies a set of transformations
  name: transformation
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-data-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-data-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Data\",\n  \"description\": \"Data is a data template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"description\": \"Source sources external data into a data template\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.DataSource\"\n    },\n    \"transformation\": {\n      \"description\": \"Transformation applies a set of transformations\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.TransformationStep\"\n      }\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"transformation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-data-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Data
---
