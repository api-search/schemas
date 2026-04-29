---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HTTPTrigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HTTPTrigger
properties_list:
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: dynamicHeaders
  type: array
- description: ''
  name: headers
  type: object
- description: ''
  name: host
  type: string
- description: ''
  name: method
  type: string
- description: Parameters is the list of key-value extracted from event's payload that are applied to the HTTP trigger resource.
  name: parameters
  type: array
- description: ''
  name: payload
  type: array
- description: ''
  name: secureHeaders
  type: array
- description: ''
  name: timeout
  type: string
- description: ''
  name: tls
  type: object
- description: URL refers to the URL to send HTTP request to.
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-http-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-http-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-http-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HTTPTrigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HTTPTrigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basicAuth\": {\n      \"title\": \"BasicAuth configuration for the http request.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth\"\n    },\n    \"dynamicHeaders\": {\n      \"type\": \"array\",\n      \"title\": \"Dynamic Headers for the request, sourced from the io.argoproj.workflow.v1alpha1. Same spec as Parameters.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\
  \n      }\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"title\": \"Headers for the HTTP request.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"title\": \"Host refers to the domain name of the server (for virtual hosting).\\n+optional\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"title\": \"Method refers to the type of the HTTP request.\\nRefer https://golang.org/src/net/http/method.go for more io.argoproj.workflow.v1alpha1.\\nDefault value is POST.\\n+optional\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters is the list of key-value extracted from event's payload that are applied to\\nthe HTTP trigger resource.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"secureHeaders\": {\n      \"type\": \"array\",\n      \"title\": \"Secure Headers stored in Kubernetes Secrets for the HTTP requests.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SecureHeader\"\n      }\n    },\n    \"timeout\": {\n      \"type\": \"string\",\n      \"title\": \"Timeout refers to the HTTP request timeout in seconds.\\nDefault value is 60 seconds.\\n+optional\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the HTTP client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"url\": {\n      \"description\": \"URL refers to the URL to send HTTP request to.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-http-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HTTPTrigger
---
