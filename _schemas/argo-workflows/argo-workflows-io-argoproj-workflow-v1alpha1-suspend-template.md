---
description: SuspendTemplate is a template subtype to suspend a workflow at a predetermined point in time
layout: schema
name: io.argoproj.workflow.v1alpha1.SuspendTemplate
properties_list:
- description: 'Duration is the seconds to wait before automatically resuming a template. Must be a string. Default unit is seconds. Could also be a Duration, e.g.: "2m", "6h"'
  name: duration
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.SuspendTemplate\",\n  \"description\": \"SuspendTemplate is a template subtype to suspend a workflow at a predetermined point in time\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"description\": \"Duration is the seconds to wait before automatically resuming a template. Must be a string. Default unit is seconds. Could also be a Duration, e.g.: \\\"2m\\\", \\\"6h\\\"\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SuspendTemplate
---
