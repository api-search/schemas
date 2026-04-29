---
description: NodeSynchronizationStatus stores the status of a node
layout: schema
name: io.argoproj.workflow.v1alpha1.NodeSynchronizationStatus
properties_list:
- description: Waiting is the name of the lock that this node is waiting for
  name: waiting
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-synchronization-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-node-synchronization-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-synchronization-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.NodeSynchronizationStatus\",\n  \"description\": \"NodeSynchronizationStatus stores the status of a node\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"waiting\": {\n      \"description\": \"Waiting is the name of the lock that this node is waiting for\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-synchronization-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.NodeSynchronizationStatus
---
