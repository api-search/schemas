---
description: ApplicationSetSyncPolicy configures how generated Applications will relate to their ApplicationSet.
layout: schema
name: v1alpha1ApplicationSetSyncPolicy
properties_list:
- description: ''
  name: applicationsSync
  type: string
- description: PreserveResourcesOnDeletion will preserve resources on deletion. If PreserveResourcesOnDeletion is set to true, these Applications will not be deleted.
  name: preserveResourcesOnDeletion
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-sync-policy-schema.json
slug: argo-cd-v1alpha1-application-set-sync-policy
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetSyncPolicy
---
