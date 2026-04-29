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
source_filename: argo-cd-v1-list-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-list-meta-schema.json\",\n  \"title\": \"v1ListMeta\",\n  \"description\": \"ListMeta describes metadata that synthetic resources must have, including lists and\\nvarious status objects. A resource may have only one of {ObjectMeta, ListMeta}.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"continue\": {\n      \"description\": \"continue may be set if the user set a limit on the number of items returned, and indicates that\\nthe server has more data available. The value is opaque and may be used to issue another request\\nto the endpoint that served this list to retrieve the next set of available objects. Continuing a\\nconsistent list may not be possible if the server configuration has changed or more than a few\\nminutes have passed. The resourceVersion field returned when using this continue\
  \ value will be\\nidentical to the value in the first response, unless you have received this token from an error\\nmessage.\",\n      \"type\": \"string\"\n    },\n    \"remainingItemCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"remainingItemCount is the number of subsequent items in the list which are not included in this\\nlist response. If the list request contained label or field selectors, then the number of\\nremaining items is unknown and the field will be left unset and omitted during serialization.\\nIf the list is complete (either because it is not chunking or because this is the last chunk),\\nthen there are no more remaining items and this field will be left unset and omitted during\\nserialization.\\nServers older than v1.15 do not set this field.\\nThe intended use of the remainingItemCount is *estimating* the size of a collection. Clients\\nshould not rely on the remainingItemCount to be set or to be exact.\\n+optional\"\n  \
  \  },\n    \"resourceVersion\": {\n      \"type\": \"string\",\n      \"title\": \"String that identifies the server's internal version of this object that\\ncan be used by clients to determine when objects have changed.\\nValue must be treated as opaque by clients and passed unmodified back to the server.\\nPopulated by the system.\\nRead-only.\\nMore info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency\\n+optional\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"title\": \"Deprecated: selfLink is a legacy read-only field that is no longer populated by the system.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-list-meta-schema.json
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
