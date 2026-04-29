---
description: ObjectReference contains enough information to let you inspect or modify the referred object.
layout: schema
name: io.k8s.api.core.v1.ObjectReference
properties_list:
- description: API version of the referent.
  name: apiVersion
  type: string
- description: If referring to a piece of an object instead of an entire object, this string should contain a valid JSON/Go field access statement, such as desiredState.manifest.containers[2]. For example, if the ob
  name: fieldPath
  type: string
- description: 'Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds'
  name: kind
  type: string
- description: 'Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names'
  name: name
  type: string
- description: 'Namespace of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/'
  name: namespace
  type: string
- description: 'Specific resourceVersion to which this reference is made, if any. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency'
  name: resourceVersion
  type: string
- description: 'UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#uids'
  name: uid
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-object-reference-schema.json
slug: argo-workflows-io-k8s-api-core-v1-object-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-object-reference-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ObjectReference\",\n  \"description\": \"ObjectReference contains enough information to let you inspect or modify the referred object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"API version of the referent.\",\n      \"type\": \"string\"\n    },\n    \"fieldPath\": {\n      \"description\": \"If referring to a piece of an object instead of an entire object, this string should contain a valid JSON/Go field access statement, such as desiredState.manifest.containers[2]. For example, if the object reference is to a container within a pod, this would take on a value like: \\\"spec.containers{name}\\\" (where \\\"name\\\" refers to the name of the container\
  \ that triggered the event) or if no container name is specified \\\"spec.containers[2]\\\" (container with index 2 in this pod). This syntax is chosen only to have some well-defined way of referencing a part of an object.\",\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"description\": \"Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/\",\n      \"type\": \"string\"\n    },\n    \"resourceVersion\": {\n      \"description\": \"Specific resourceVersion to which this reference is made, if any. More info:\
  \ https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency\",\n      \"type\": \"string\"\n    },\n    \"uid\": {\n      \"description\": \"UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#uids\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-object-reference-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ObjectReference
---
