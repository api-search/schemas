---
description: ListMeta describes metadata that synthetic resources must have, including lists and various status objects. A resource may have only one of {ObjectMeta, ListMeta}.
layout: schema
name: v1ListMeta
properties_list:
- description: 'continue may be set if the user set a limit on the number of items returned, and indicates that the server has more data available. The value is opaque and may be used to issue another request to the '
  name: continue
  type: string
- description: ''
  name: remainingItemCount
  type: integer
- description: ''
  name: resourceVersion
  type: string
- description: ''
  name: selfLink
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-list-meta-schema.json
slug: argo-cd-v1-list-meta
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1ListMeta
---
