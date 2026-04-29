---
description: MicroTime is version of Time with microsecond level precision. +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false
layout: schema
name: v1MicroTime
properties_list:
- description: Non-negative fractions of a second at nanosecond resolution. Negative second values with fractions must still have non-negative nanos values that count forward in time. Must be from 0 to 999,999,999 i
  name: nanos
  type: integer
- description: Represents seconds of UTC time since Unix epoch 1970-01-01T00:00:00Z. Must be from 0001-01-01T00:00:00Z to 9999-12-31T23:59:59Z inclusive.
  name: seconds
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-micro-time-schema.json
slug: argo-cd-v1-micro-time
source_filename: argo-cd-v1-micro-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-micro-time-schema.json\",\n  \"title\": \"v1MicroTime\",\n  \"description\": \"MicroTime is version of Time with microsecond level precision.\\n\\n+protobuf.options.marshal=false\\n+protobuf.as=Timestamp\\n+protobuf.options.(gogoproto.goproto_stringer)=false\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nanos\": {\n      \"description\": \"Non-negative fractions of a second at nanosecond resolution. Negative\\nsecond values with fractions must still have non-negative nanos values\\nthat count forward in time. Must be from 0 to 999,999,999\\ninclusive. This field may be limited in precision depending on context.\",\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"seconds\": {\n      \"description\": \"Represents seconds of UTC time since Unix epoch\\n1970-01-01T00:00:00Z.\
  \ Must be from 0001-01-01T00:00:00Z to\\n9999-12-31T23:59:59Z inclusive.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-micro-time-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1MicroTime
---
