---
description: HTTPGetAction describes an action based on HTTP Get requests.
layout: schema
name: io.k8s.api.core.v1.HTTPGetAction
properties_list:
- description: Host name to connect to, defaults to the pod IP. You probably want to set "Host" in httpHeaders instead.
  name: host
  type: string
- description: Custom headers to set in the request. HTTP allows repeated headers.
  name: httpHeaders
  type: array
- description: Path to access on the HTTP server.
  name: path
  type: string
- description: Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME.
  name: port
  type: object
- description: Scheme to use for connecting to the host. Defaults to HTTP.
  name: scheme
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-http-get-action-schema.json
slug: argo-workflows-io-k8s-api-core-v1-http-get-action
source_filename: argo-workflows-io-k8s-api-core-v1-http-get-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-http-get-action-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.HTTPGetAction\",\n  \"description\": \"HTTPGetAction describes an action based on HTTP Get requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"description\": \"Host name to connect to, defaults to the pod IP. You probably want to set \\\"Host\\\" in httpHeaders instead.\",\n      \"type\": \"string\"\n    },\n    \"httpHeaders\": {\n      \"description\": \"Custom headers to set in the request. HTTP allows repeated headers.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.HTTPHeader\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"path\": {\n      \"description\": \"Path to access on the HTTP server.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"description\": \"Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    },\n    \"scheme\": {\n      \"description\": \"Scheme to use for connecting to the host. Defaults to HTTP.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"port\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-http-get-action-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.HTTPGetAction
---
