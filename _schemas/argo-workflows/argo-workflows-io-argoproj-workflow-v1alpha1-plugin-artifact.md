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
