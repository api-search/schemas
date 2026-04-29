---
description: Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON. Wrappers are provided for many of the factory methods that the time package offers. +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false
layout: schema
name: v1Time
properties_list: []
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-time-schema.json
slug: argo-cd-v1-time
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-time-schema.json\",\n  \"title\": \"v1Time\",\n  \"description\": \"Time is a wrapper around time.Time which supports correct\\nmarshaling to YAML and JSON.  Wrappers are provided for many\\nof the factory methods that the time package offers.\\n\\n+protobuf.options.marshal=false\\n+protobuf.as=Timestamp\\n+protobuf.options.(gogoproto.goproto_stringer)=false\",\n  \"type\": \"string\",\n  \"format\": \"date-time\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-time-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1Time
---
