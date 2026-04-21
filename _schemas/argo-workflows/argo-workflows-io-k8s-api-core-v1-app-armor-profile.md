---
description: AppArmorProfile defines a pod or container's AppArmor settings.
layout: schema
name: io.k8s.api.core.v1.AppArmorProfile
properties_list:
- description: localhostProfile indicates a profile loaded on the node that should be used. The profile must be preconfigured on the node to work. Must match the loaded name of the profile. Must be set if and only i
  name: localhostProfile
  type: string
- description: 'type indicates which kind of AppArmor profile will be applied. Valid options are: Localhost - a profile pre-loaded on the node. RuntimeDefault - the container runtime''s default profile. Unconfined - n'
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-app-armor-profile-schema.json
slug: argo-workflows-io-k8s-api-core-v1-app-armor-profile
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.AppArmorProfile
---
