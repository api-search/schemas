---
description: Route port configuration that specifies which service port the route points to.
layout: schema
name: RoutePort
properties_list:
- description: The target port on pods selected by the service this route points to. Can be a port name or number.
  name: targetPort
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-route-port-schema.json
slug: openshift-rest-route-port
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoutePort\",\n  \"type\": \"object\",\n  \"description\": \"Route port configuration that specifies which service port the route points to.\",\n  \"properties\": {\n    \"targetPort\": {\n      \"type\": \"string\",\n      \"description\": \"The target port on pods selected by the service this route points to. Can be a port name or number.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-route-port-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RoutePort
---
