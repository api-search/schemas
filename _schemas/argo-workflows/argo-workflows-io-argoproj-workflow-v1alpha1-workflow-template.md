---
description: WorkflowTemplate is the definition of a workflow template resource
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowTemplate
properties_list:
- description: 'APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: http'
  name: apiVersion
  type: string
- description: 'Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https'
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowTemplate\",\n  \"description\": \"WorkflowTemplate is the definition of a workflow template resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.io.k8s.community/contributors/devel/sig-architecture/api-conventions.md#resources\",\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"description\": \"Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint\
  \ the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.io.k8s.community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta\"\n    },\n    \"spec\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowSpec\"\n    }\n  },\n  \"required\": [\n    \"metadata\",\n    \"spec\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowTemplate
---
