---
description: io.argoproj.workflow.v1alpha1.HTTP schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.HTTP
properties_list:
- description: Body is content of the HTTP Request
  name: body
  type: string
- description: BodyFrom is content of the HTTP Request as Bytes
  name: bodyFrom
  type: object
- description: Headers are an optional list of headers to send with HTTP requests
  name: headers
  type: array
- description: InsecureSkipVerify is a bool when if set to true will skip TLS verification for the HTTP client
  name: insecureSkipVerify
  type: boolean
- description: Method is HTTP methods for HTTP Request
  name: method
  type: string
- description: SuccessCondition is an expression if evaluated to true is considered successful
  name: successCondition
  type: string
- description: TimeoutSeconds is request timeout for HTTP Request. Default is 30 seconds
  name: timeoutSeconds
  type: integer
- description: URL of the HTTP Request
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-http
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.HTTP\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.HTTP schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"description\": \"Body is content of the HTTP Request\",\n      \"type\": \"string\"\n    },\n    \"bodyFrom\": {\n      \"description\": \"BodyFrom is  content of the HTTP Request as Bytes\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HTTPBodySource\"\n    },\n    \"headers\": {\n      \"description\": \"Headers are an optional list of headers to send with HTTP requests\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HTTPHeader\"\n      }\n\
  \    },\n    \"insecureSkipVerify\": {\n      \"description\": \"InsecureSkipVerify is a bool when if set to true will skip TLS verification for the HTTP client\",\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"description\": \"Method is HTTP methods for HTTP Request\",\n      \"type\": \"string\"\n    },\n    \"successCondition\": {\n      \"description\": \"SuccessCondition is an expression if evaluated to true is considered successful\",\n      \"type\": \"string\"\n    },\n    \"timeoutSeconds\": {\n      \"description\": \"TimeoutSeconds is request timeout for HTTP Request. Default is 30 seconds\",\n      \"type\": \"integer\"\n    },\n    \"url\": {\n      \"description\": \"URL of the HTTP Request\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HTTP
---
