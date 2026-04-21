---
description: v1alpha1ResourceOverride schema from Argo CD API
layout: schema
name: v1alpha1ResourceOverride
properties_list:
- description: Actions defines the set of actions that can be performed on the resource, as a Lua script.
  name: actions
  type: string
- description: HealthLua contains a Lua script that defines custom health checks for the resource.
  name: healthLua
  type: string
- description: ''
  name: ignoreDifferences
  type: object
- description: ''
  name: ignoreResourceUpdates
  type: object
- description: KnownTypeFields lists fields for which unit conversions should be applied.
  name: knownTypeFields
  type: array
- description: UseOpenLibs indicates whether to use open-source libraries for the resource.
  name: useOpenLibs
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-override-schema.json
slug: argo-cd-v1alpha1-resource-override
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceOverride
---
