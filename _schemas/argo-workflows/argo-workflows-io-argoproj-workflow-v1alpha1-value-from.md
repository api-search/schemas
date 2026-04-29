---
description: ValueFrom describes a location in which to obtain the value to a parameter
layout: schema
name: io.argoproj.workflow.v1alpha1.ValueFrom
properties_list:
- description: ConfigMapKeyRef is configmap selector for input parameter configuration
  name: configMapKeyRef
  type: object
- description: Default specifies a value to be used if retrieving the value from the specified source fails
  name: default
  type: string
- description: Selector (https://github.com/expr-lang/expr) that is evaluated against the event to get the value of the parameter. E.g. `payload.message`
  name: event
  type: string
- description: Expression, if defined, is evaluated to specify the value for the parameter
  name: expression
  type: string
- description: JQFilter expression against the resource object in resource templates
  name: jqFilter
  type: string
- description: JSONPath of a resource to retrieve an output parameter value from in resource templates
  name: jsonPath
  type: string
- description: Parameter reference to a step or dag task in which to retrieve an output parameter value from (e.g. '{{steps.mystep.outputs.myparam}}')
  name: parameter
  type: string
- description: Path in the container to retrieve an output parameter value from in container templates
  name: path
  type: string
- description: Supplied value to be filled in directly, either through the CLI, API, etc.
  name: supplied
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-value-from-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-value-from
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-value-from-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ValueFrom\",\n  \"description\": \"ValueFrom describes a location in which to obtain the value to a parameter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapKeyRef\": {\n      \"description\": \"ConfigMapKeyRef is configmap selector for input parameter configuration\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapKeySelector\"\n    },\n    \"default\": {\n      \"description\": \"Default specifies a value to be used if retrieving the value from the specified source fails\",\n      \"type\": \"string\"\n    },\n    \"event\": {\n      \"description\": \"Selector (https://github.com/expr-lang/expr) that is evaluated against the event to get the value of the\
  \ parameter. E.g. `payload.message`\",\n      \"type\": \"string\"\n    },\n    \"expression\": {\n      \"description\": \"Expression, if defined, is evaluated to specify the value for the parameter\",\n      \"type\": \"string\"\n    },\n    \"jqFilter\": {\n      \"description\": \"JQFilter expression against the resource object in resource templates\",\n      \"type\": \"string\"\n    },\n    \"jsonPath\": {\n      \"description\": \"JSONPath of a resource to retrieve an output parameter value from in resource templates\",\n      \"type\": \"string\"\n    },\n    \"parameter\": {\n      \"description\": \"Parameter reference to a step or dag task in which to retrieve an output parameter value from (e.g. '{{steps.mystep.outputs.myparam}}')\",\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"description\": \"Path in the container to retrieve an output parameter value from in container templates\",\n      \"type\": \"string\"\n    },\n    \"supplied\": {\n      \"description\"\
  : \"Supplied value to be filled in directly, either through the CLI, API, etc.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SuppliedValueFrom\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-value-from-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ValueFrom
---
