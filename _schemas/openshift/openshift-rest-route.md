---
description: A Route exposes a service at a hostname, enabling external access to applications in the cluster. Routes support TLS termination strategies including edge, passthrough, and re-encrypt.
layout: schema
name: Route
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-route-schema.json
slug: openshift-rest-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Route\",\n  \"type\": \"object\",\n  \"description\": \"A Route exposes a service at a hostname, enabling external access to applications in the cluster. Routes support TLS termination strategies including edge, passthrough, and re-encrypt.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-route-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Route
---
