---
description: Specifies the target that traffic is routed to. Weight controls the proportion of traffic sent to this backend.
layout: schema
name: RouteTargetReference
properties_list:
- description: The kind of target, typically Service.
  name: kind
  type: string
- description: Name of the target service.
  name: name
  type: string
- description: Relative weight for traffic distribution (0-256). A zero weight causes no traffic to be sent to this backend.
  name: weight
  type: integer
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-route-target-reference-schema.json
slug: openshift-rest-route-target-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteTargetReference\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the target that traffic is routed to. Weight controls the proportion of traffic sent to this backend.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of target, typically Service.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target service.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Relative weight for traffic distribution (0-256). A zero weight causes no traffic to be sent to this backend.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-route-target-reference-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RouteTargetReference
---
