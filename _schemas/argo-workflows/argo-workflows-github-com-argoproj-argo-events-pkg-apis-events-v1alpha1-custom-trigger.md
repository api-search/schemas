---
description: CustomTrigger refers to the specification of the custom trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CustomTrigger
properties_list:
- description: CertSecret refers to the secret that contains cert for secure connection between sensor and custom trigger gRPC server.
  name: certSecret
  type: object
- description: Parameters is the list of parameters that is applied to resolved custom trigger trigger object.
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: secure
  type: boolean
- description: ServerNameOverride for the secure connection between sensor and custom trigger gRPC server.
  name: serverNameOverride
  type: string
- description: ''
  name: serverURL
  type: string
- description: Spec is the custom trigger resource specification that custom trigger gRPC server knows how to interpret.
  name: spec
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CustomTrigger\",\n  \"description\": \"CustomTrigger refers to the specification of the custom trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certSecret\": {\n      \"description\": \"CertSecret refers to the secret that contains cert for secure connection between sensor and custom trigger gRPC server.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters is the list of parameters that is applied to resolved custom trigger trigger object.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\
  \n      }\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value extracted from an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"secure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Secure refers to type of the connection between sensor to custom trigger gRPC\"\n    },\n    \"serverNameOverride\": {\n      \"description\": \"ServerNameOverride for the secure connection between sensor and custom trigger gRPC server.\",\n      \"type\": \"string\"\n    },\n    \"serverURL\": {\n      \"type\": \"string\",\n      \"title\": \"ServerURL is the url of the gRPC server that executes custom trigger\"\n    },\n    \"spec\": {\n      \"description\": \"Spec is the custom trigger resource specification that custom trigger gRPC server knows how to interpret.\",\n      \"type\"\
  : \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CustomTrigger
---
