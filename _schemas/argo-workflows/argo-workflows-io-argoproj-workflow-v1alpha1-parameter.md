---
description: Parameter indicate a passed string parameter to a service template with an optional default value
layout: schema
name: io.argoproj.workflow.v1alpha1.Parameter
properties_list:
- description: Default is the default value to use for an input parameter if a value was not supplied
  name: default
  type: string
- description: Description is the parameter description
  name: description
  type: string
- description: Enum holds a list of string values to choose from, for the actual value of the parameter
  name: enum
  type: array
- description: GlobalName exports an output parameter to the global scope, making it available as '{{io.argoproj.workflow.v1alpha1.outputs.parameters.XXXX}} and in workflow.status.outputs.parameters
  name: globalName
  type: string
- description: Name is the parameter name
  name: name
  type: string
- description: Value is the literal value to use for the parameter. If specified in the context of an input parameter, any passed values take precedence over the specified value
  name: value
  type: string
- description: ValueFrom is the source for the output parameter's value
  name: valueFrom
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-parameter-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-parameter-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Parameter\",\n  \"description\": \"Parameter indicate a passed string parameter to a service template with an optional default value\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default\": {\n      \"description\": \"Default is the default value to use for an input parameter if a value was not supplied\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Description is the parameter description\",\n      \"type\": \"string\"\n    },\n    \"enum\": {\n      \"description\": \"Enum holds a list of string values to choose from, for the actual value of the parameter\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n\
  \      }\n    },\n    \"globalName\": {\n      \"description\": \"GlobalName exports an output parameter to the global scope, making it available as '{{io.argoproj.workflow.v1alpha1.outputs.parameters.XXXX}} and in workflow.status.outputs.parameters\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name is the parameter name\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Value is the literal value to use for the parameter. If specified in the context of an input parameter, any passed values take precedence over the specified value\",\n      \"type\": \"string\"\n    },\n    \"valueFrom\": {\n      \"description\": \"ValueFrom is the source for the output parameter's value\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ValueFrom\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-parameter-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Parameter
---
