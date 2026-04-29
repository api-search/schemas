---
description: TypedObjectReference contains enough information to let you locate the typed referenced object
layout: schema
name: io.k8s.api.core.v1.TypedObjectReference
properties_list:
- description: APIGroup is the group for the resource being referenced. If APIGroup is not specified, the specified Kind must be in the core API group. For any other third-party types, APIGroup is required.
  name: apiGroup
  type: string
- description: Kind is the type of resource being referenced
  name: kind
  type: string
- description: Name is the name of resource being referenced
  name: name
  type: string
- description: Namespace is the namespace of resource being referenced Note that when a namespace is specified, a gateway.networking.k8s.io/ReferenceGrant object is required in the referent namespace to allow that n
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-typed-object-reference-schema.json
slug: argo-workflows-io-k8s-api-core-v1-typed-object-reference
source_filename: argo-workflows-io-k8s-api-core-v1-typed-object-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-typed-object-reference-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.TypedObjectReference\",\n  \"description\": \"TypedObjectReference contains enough information to let you locate the typed referenced object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiGroup\": {\n      \"description\": \"APIGroup is the group for the resource being referenced. If APIGroup is not specified, the specified Kind must be in the core API group. For any other third-party types, APIGroup is required.\",\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"description\": \"Kind is the type of resource being referenced\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name is the name of resource being referenced\",\n      \"type\": \"\
  string\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace is the namespace of resource being referenced Note that when a namespace is specified, a gateway.networking.k8s.io/ReferenceGrant object is required in the referent namespace to allow that namespace's owner to accept the reference. See the ReferenceGrant documentation for details. (Alpha) This field requires the CrossNamespaceVolumeDataSource feature gate to be enabled.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-typed-object-reference-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.TypedObjectReference
---
