---
description: TTLStrategy is the strategy for the time to live depending on if the workflow succeeded or failed
layout: schema
name: io.argoproj.workflow.v1alpha1.TTLStrategy
properties_list:
- description: SecondsAfterCompletion is the number of seconds to live after completion
  name: secondsAfterCompletion
  type: integer
- description: SecondsAfterFailure is the number of seconds to live after failure
  name: secondsAfterFailure
  type: integer
- description: SecondsAfterSuccess is the number of seconds to live after success
  name: secondsAfterSuccess
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.TTLStrategy\",\n  \"description\": \"TTLStrategy is the strategy for the time to live depending on if the workflow succeeded or failed\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"secondsAfterCompletion\": {\n      \"description\": \"SecondsAfterCompletion is the number of seconds to live after completion\",\n      \"type\": \"integer\"\n    },\n    \"secondsAfterFailure\": {\n      \"description\": \"SecondsAfterFailure is the number of seconds to live after failure\",\n      \"type\": \"integer\"\n    },\n    \"secondsAfterSuccess\": {\n      \"description\": \"SecondsAfterSuccess is the number of seconds to live after success\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.TTLStrategy
---
