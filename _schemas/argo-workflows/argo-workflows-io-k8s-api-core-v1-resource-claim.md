---
description: ResourceClaim references one entry in PodSpec.ResourceClaims.
layout: schema
name: io.k8s.api.core.v1.ResourceClaim
properties_list:
- description: Name must match the name of one entry in pod.spec.resourceClaims of the Pod where this field is used. It makes that resource available inside a container.
  name: name
  type: string
- description: Request is the name chosen for a request in the referenced claim. If empty, everything from the claim is made available, otherwise only the result of this request.
  name: request
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-resource-claim-schema.json
slug: argo-workflows-io-k8s-api-core-v1-resource-claim
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ResourceClaim
---
