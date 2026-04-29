---
description: Current state of the Route.
layout: schema
name: RouteStatus
properties_list:
- description: Status entries for each router that has admitted the route.
  name: ingress
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-route-status-schema.json
slug: openshift-rest-route-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteStatus\",\n  \"type\": \"object\",\n  \"description\": \"Current state of the Route.\",\n  \"properties\": {\n    \"ingress\": {\n      \"type\": \"array\",\n      \"description\": \"Status entries for each router that has admitted the route.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-route-status-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RouteStatus
---
