---
description: PluginGenerator defines connection info specific to Plugin.
layout: schema
name: v1alpha1PluginGenerator
properties_list:
- description: ''
  name: configMapRef
  type: object
- description: ''
  name: input
  type: object
- description: RequeueAfterSeconds determines how long the ApplicationSet controller will wait before reconciling the ApplicationSet again.
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: template
  type: object
- description: Values contains key/value pairs which are passed directly as parameters to the template. These values will not be sent as parameters to the plugin.
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-plugin-generator-schema.json
slug: argo-cd-v1alpha1-plugin-generator
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PluginGenerator
---
