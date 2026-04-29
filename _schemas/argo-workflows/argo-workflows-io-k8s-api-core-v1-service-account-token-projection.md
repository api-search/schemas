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
source_filename: argo-workflows-io-k8s-api-core-v1-service-account-token-projection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-service-account-token-projection-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ServiceAccountTokenProjection\",\n  \"description\": \"ServiceAccountTokenProjection represents a projected service account token volume. This projection can be used to insert a service account token into the pods runtime filesystem for use against APIs (Kubernetes API Server or otherwise).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"audience\": {\n      \"description\": \"audience is the intended audience of the token. A recipient of a token must identify itself with an identifier specified in the audience of the token, and otherwise should reject the token. The audience defaults to the identifier of the apiserver.\",\n      \"type\": \"string\"\n    },\n    \"expirationSeconds\"\
  : {\n      \"description\": \"expirationSeconds is the requested duration of validity of the service account token. As the token approaches expiration, the kubelet volume plugin will proactively rotate the service account token. The kubelet will start trying to rotate the token if the token is older than 80 percent of its time to live or if the token is older than 24 hours.Defaults to 1 hour and must be at least 10 minutes.\",\n      \"type\": \"integer\"\n    },\n    \"path\": {\n      \"description\": \"path is the path relative to the mount point of the file to project the token into.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-service-account-token-projection-schema.json
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
