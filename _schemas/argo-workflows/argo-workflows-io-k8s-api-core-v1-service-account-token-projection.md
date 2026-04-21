---
description: ServiceAccountTokenProjection represents a projected service account token volume. This projection can be used to insert a service account token into the pods runtime filesystem for use against APIs (Kubernetes API Server or otherwise).
layout: schema
name: io.k8s.api.core.v1.ServiceAccountTokenProjection
properties_list:
- description: audience is the intended audience of the token. A recipient of a token must identify itself with an identifier specified in the audience of the token, and otherwise should reject the token. The audien
  name: audience
  type: string
- description: expirationSeconds is the requested duration of validity of the service account token. As the token approaches expiration, the kubelet volume plugin will proactively rotate the service account token. T
  name: expirationSeconds
  type: integer
- description: path is the path relative to the mount point of the file to project the token into.
  name: path
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-service-account-token-projection-schema.json
slug: argo-workflows-io-k8s-api-core-v1-service-account-token-projection
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ServiceAccountTokenProjection
---
