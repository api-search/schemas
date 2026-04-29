---
description: 'ObjectReference contains enough information to let you inspect or modify the referred object. --- New uses of this type are discouraged because of difficulty describing its usage when embedded in APIs. 1. Ignored fields. It includes many fields which are not generally honored. For instance, ResourceVersion and FieldPath are both very rarely valid in actual usage. 2. Invalid usage help. It is impossible to add specific help for individual usage. In most embedded usages, there are particular restrictions like, "must refer only to types A and B" or "UID not honored" or "name must be restricted". Those cannot be well described when embedded. 3. Inconsistent validation. Because the usages are different, the validation rules are different by usage, which makes it hard for users to predict what will happen. 4. The fields are both imprecise and overly precise. Kind is not a precise mapping to a URL. This can produce ambiguity during interpretation and require a REST mapping. In most
  cases, the dependency is on the group,resource tuple and the version of the actual struct is irrelevant. 5. We cannot easily change it. Because this type is embedded in many locations, updates to this type will affect numerous schemas. Don''t make new APIs embed an underspecified API type they do not control. Instead of using this type, create a locally provided and used type that is well-focused on your reference. For example, ServiceReferences for admission registration: https://github.com/kubernetes/api/blob/release-1.17/admissionregistration/v1/types.go#L533 . +k8s:deepcopy-gen:interfaces=k8s.io/apimachinery/pkg/runtime.Object +structType=atomic'
layout: schema
name: v1ObjectReference
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: fieldPath
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: resourceVersion
  type: string
- description: ''
  name: uid
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-object-reference-schema.json
slug: argo-cd-v1-object-reference
source_filename: argo-cd-v1-object-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-object-reference-schema.json\",\n  \"title\": \"v1ObjectReference\",\n  \"description\": \"ObjectReference contains enough information to let you inspect or modify the referred object.\\n---\\nNew uses of this type are discouraged because of difficulty describing its usage when embedded in APIs.\\n 1. Ignored fields.  It includes many fields which are not generally honored.  For instance, ResourceVersion and FieldPath are both very rarely valid in actual usage.\\n 2. Invalid usage help.  It is impossible to add specific help for individual usage.  In most embedded usages, there are particular\\n    restrictions like, \\\"must refer only to types A and B\\\" or \\\"UID not honored\\\" or \\\"name must be restricted\\\".\\n    Those cannot be well described when embedded.\\n 3. Inconsistent validation.\
  \  Because the usages are different, the validation rules are different by usage, which makes it hard for users to predict what will happen.\\n 4. The fields are both imprecise and overly precise.  Kind is not a precise mapping to a URL. This can produce ambiguity\\n    during interpretation and require a REST mapping.  In most cases, the dependency is on the group,resource tuple\\n    and the version of the actual struct is irrelevant.\\n 5. We cannot easily change it.  Because this type is embedded in many locations, updates to this type\\n    will affect numerous schemas.  Don't make new APIs embed an underspecified API type they do not control.\\n\\nInstead of using this type, create a locally provided and used type that is well-focused on your reference.\\nFor example, ServiceReferences for admission registration: https://github.com/kubernetes/api/blob/release-1.17/admissionregistration/v1/types.go#L533 .\\n+k8s:deepcopy-gen:interfaces=k8s.io/apimachinery/pkg/runtime.Object\\n+structType=atomic\"\
  ,\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"title\": \"API version of the referent.\\n+optional\"\n    },\n    \"fieldPath\": {\n      \"type\": \"string\",\n      \"title\": \"If referring to a piece of an object instead of an entire object, this string\\nshould contain a valid JSON/Go field access statement, such as desiredState.manifest.containers[2].\\nFor example, if the object reference is to a container within a pod, this would take on a value like:\\n\\\"spec.containers{name}\\\" (where \\\"name\\\" refers to the name of the container that triggered\\nthe event) or if no container name is specified \\\"spec.containers[2]\\\" (container with\\nindex 2 in this pod). This syntax is chosen only to have some well-defined way of\\nreferencing a part of an object.\\nTODO: this design is not final and this field is subject to change in the future.\\n+optional\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n     \
  \ \"title\": \"Kind of the referent.\\nMore info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\\n+optional\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name of the referent.\\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names\\n+optional\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"title\": \"Namespace of the referent.\\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/\\n+optional\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\",\n      \"title\": \"Specific resourceVersion to which this reference is made, if any.\\nMore info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency\\n+optional\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"title\": \"UID of the referent.\\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#uids\\\
  n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-object-reference-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1ObjectReference
---
