---
description: Describes the state of a route at a point in time.
layout: schema
name: RouteIngressCondition
properties_list:
- description: The type of the condition (e.g., Admitted).
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: reason
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: lastTransitionTime
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-route-ingress-condition-schema.json
slug: openshift-rest-route-ingress-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteIngressCondition\",\n  \"type\": \"object\",\n  \"description\": \"Describes the state of a route at a point in time.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the condition (e.g., Admitted).\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"lastTransitionTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-route-ingress-condition-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RouteIngressCondition
---
