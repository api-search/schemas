---
description: 'WorkflowStep is a reference to a template to execute in a series of step Note: CEL validation cannot check withItems (Schemaless) or inline (PreserveUnknownFields) fields.'
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowStep
properties_list:
- description: Arguments hold arguments to the template
  name: arguments
  type: object
- description: ContinueOn makes argo to proceed with the following step even if this step fails. Errors and Failed states can be specified
  name: continueOn
  type: object
- description: Hooks holds the lifecycle hook which is invoked at lifecycle of step, irrespective of the success, failure, or error status of the primary step
  name: hooks
  type: object
- description: 'Inline is the template. Template must be empty if this is declared (and vice-versa). Note: This struct is defined recursively, since the inline template can potentially contain steps/DAGs that also ha'
  name: inline
  type: object
- description: Name of the step
  name: name
  type: string
- description: 'OnExit is a template reference which is invoked at the end of the template, irrespective of the success, failure, or error of the primary template. Deprecated: Use Hooks[exit].Template instead.'
  name: onExit
  type: string
- description: Template is the name of the template to execute as the step
  name: template
  type: string
- description: TemplateRef is the reference to the template resource to execute as the step.
  name: templateRef
  type: object
- description: When is an expression in which the step should conditionally execute
  name: when
  type: string
- description: 'WithItems expands a step into multiple parallel steps from the items in the list Note: The structure of WithItems is free-form, so we need "x-kubernetes-preserve-unknown-fields: true" in the validatio'
  name: withItems
  type: array
- description: WithParam expands a step into multiple parallel steps from the value in the parameter, which is expected to be a JSON list.
  name: withParam
  type: string
- description: WithSequence expands a step into a numeric sequence
  name: withSequence
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-step-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-step
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-step-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowStep\",\n  \"description\": \"WorkflowStep is a reference to a template to execute in a series of step Note: CEL validation cannot check withItems (Schemaless) or inline (PreserveUnknownFields) fields.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arguments\": {\n      \"description\": \"Arguments hold arguments to the template\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Arguments\"\n    },\n    \"continueOn\": {\n      \"description\": \"ContinueOn makes argo to proceed with the following step even if this step fails. Errors and Failed states can be specified\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ContinueOn\"\n    },\n\
  \    \"hooks\": {\n      \"description\": \"Hooks holds the lifecycle hook which is invoked at lifecycle of step, irrespective of the success, failure, or error status of the primary step\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.LifecycleHook\"\n      }\n    },\n    \"inline\": {\n      \"description\": \"Inline is the template. Template must be empty if this is declared (and vice-versa). Note: This struct is defined recursively, since the inline template can potentially contain steps/DAGs that also has an \\\"inline\\\" field. Kubernetes doesn't allow recursive types, so we need \\\"x-kubernetes-preserve-unknown-fields: true\\\" in the validation schema.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Template\"\n    },\n    \"name\": {\n      \"description\": \"Name of the step\",\n      \"type\": \"string\"\n    },\n    \"onExit\": {\n      \"description\": \"OnExit is a template\
  \ reference which is invoked at the end of the template, irrespective of the success, failure, or error of the primary template.\\n\\nDeprecated: Use Hooks[exit].Template instead.\",\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"description\": \"Template is the name of the template to execute as the step\",\n      \"type\": \"string\"\n    },\n    \"templateRef\": {\n      \"description\": \"TemplateRef is the reference to the template resource to execute as the step.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.TemplateRef\"\n    },\n    \"when\": {\n      \"description\": \"When is an expression in which the step should conditionally execute\",\n      \"type\": \"string\"\n    },\n    \"withItems\": {\n      \"description\": \"WithItems expands a step into multiple parallel steps from the items in the list Note: The structure of WithItems is free-form, so we need \\\"x-kubernetes-preserve-unknown-fields: true\\\" in the validation schema.\",\n\
  \      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Item\"\n      }\n    },\n    \"withParam\": {\n      \"description\": \"WithParam expands a step into multiple parallel steps from the value in the parameter, which is expected to be a JSON list.\",\n      \"type\": \"string\"\n    },\n    \"withSequence\": {\n      \"description\": \"WithSequence expands a step into a numeric sequence\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Sequence\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-step-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowStep
---
