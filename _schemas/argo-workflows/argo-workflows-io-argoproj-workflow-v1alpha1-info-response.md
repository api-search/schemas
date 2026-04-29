---
description: io.argoproj.workflow.v1alpha1.InfoResponse schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.InfoResponse
properties_list:
- description: ''
  name: columns
  type: array
- description: ''
  name: links
  type: array
- description: ''
  name: managedNamespace
  type: string
- description: ''
  name: modals
  type: object
- description: ''
  name: navColor
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-info-response-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-info-response-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.InfoResponse\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.InfoResponse schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"columns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Column\"\n      }\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Link\"\n      }\n    },\n    \"managedNamespace\": {\n      \"type\": \"string\"\n    },\n    \"modals\": {\n      \"type\": \"object\",\n      \"title\": \"which modals to show\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\
  \n      }\n    },\n    \"navColor\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-info-response-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.InfoResponse
---
