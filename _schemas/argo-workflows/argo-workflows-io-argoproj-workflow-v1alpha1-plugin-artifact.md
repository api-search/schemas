---
description: PluginArtifact is the location of a plugin artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.PluginArtifact
properties_list:
- description: Configuration is the plugin defined configuration for the artifact driver plugin
  name: configuration
  type: string
- description: ConnectionTimeoutSeconds is the timeout for the artifact driver connection, overriding the driver's timeout
  name: connectionTimeoutSeconds
  type: integer
- description: Key is the path in the artifact repository where the artifact resides
  name: key
  type: string
- description: Name is the name of the artifact driver plugin
  name: name
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.PluginArtifact\",\n  \"description\": \"PluginArtifact is the location of a plugin artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"description\": \"Configuration is the plugin defined configuration for the artifact driver plugin\",\n      \"type\": \"string\"\n    },\n    \"connectionTimeoutSeconds\": {\n      \"description\": \"ConnectionTimeoutSeconds is the timeout for the artifact driver connection, overriding the driver's timeout\",\n      \"type\": \"integer\"\n    },\n    \"key\": {\n      \"description\": \"Key is the path in the artifact repository where the artifact resides\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n\
  \      \"description\": \"Name is the name of the artifact driver plugin\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.PluginArtifact
---
