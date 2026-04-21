---
description: ListMeta describes metadata that synthetic resources must have, including lists and various status objects. A resource may have only one of {ObjectMeta, ListMeta}.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.ListMeta
properties_list:
- description: 'continue may be set if the user set a limit on the number of items returned, and indicates that the server has more data available. The value is opaque and may be used to issue another request to the '
  name: continue
  type: string
- description: remainingItemCount is the number of subsequent items in the list which are not included in this list response. If the list request contained label or field selectors, then the number of remaining item
  name: remainingItemCount
  type: integer
- description: String that identifies the server's internal version of this object that can be used by clients to determine when objects have changed. Value must be treated as opaque by clients and passed unmodified
  name: resourceVersion
  type: string
- description: 'Deprecated: selfLink is a legacy read-only field that is no longer populated by the system.'
  name: selfLink
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-list-meta-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-list-meta
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.ListMeta
---
