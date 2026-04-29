---
description: Holds information about the places where a route is exposed.
layout: schema
name: RouteIngress
properties_list:
- description: The hostname assigned to the route by the router.
  name: host
  type: string
- description: The name of the router that admitted this route.
  name: routerName
  type: string
- description: ''
  name: conditions
  type: array
- description: The wildcard policy applied by the router.
  name: wildcardPolicy
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-route-ingress-schema.json
slug: openshift-rest-route-ingress
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteIngress\",\n  \"type\": \"object\",\n  \"description\": \"Holds information about the places where a route is exposed.\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname assigned to the route by the router.\"\n    },\n    \"routerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the router that admitted this route.\"\n    },\n    \"conditions\": {\n      \"type\": \"array\"\n    },\n    \"wildcardPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The wildcard policy applied by the router.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-route-ingress-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RouteIngress
---
