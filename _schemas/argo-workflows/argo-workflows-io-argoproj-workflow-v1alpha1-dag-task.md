---
description: 'DAGTask represents a node in the graph during DAG execution Note: CEL validation cannot check withItems (Schemaless) or inline (PreserveUnknownFields) fields.'
layout: schema
name: io.argoproj.workflow.v1alpha1.DAGTask
properties_list:
- description: Arguments are the parameter and artifact arguments to the template
  name: arguments
  type: object
- description: ContinueOn makes argo to proceed with the following step even if this step fails. Errors and Failed states can be specified
  name: continueOn
  type: object
- description: Dependencies are name of other targets which this depends on
  name: dependencies
  type: array
- description: Depends are name of other targets which this depends on
  name: depends
  type: string
- description: Hooks hold the lifecycle hook which is invoked at lifecycle of task, irrespective of the success, failure, or error status of the primary task
  name: hooks
  type: object
- description: 'Inline is the template. Template must be empty if this is declared (and vice-versa). Note: As mentioned in the corresponding definition in WorkflowStep, this struct is defined recursively, so we need '
  name: inline
  type: object
- description: Name is the name of the target
  name: name
  type: string
- description: 'OnExit is a template reference which is invoked at the end of the template, irrespective of the success, failure, or error of the primary template. Deprecated: Use Hooks[exit].Template instead.'
  name: onExit
  type: string
- description: Name of template to execute
  name: template
  type: string
- description: TemplateRef is the reference to the template resource to execute.
  name: templateRef
  type: object
- description: When is an expression in which the task should conditionally execute
  name: when
  type: string
- description: 'WithItems expands a task into multiple parallel tasks from the items in the list Note: The structure of WithItems is free-form, so we need "x-kubernetes-preserve-unknown-fields: true" in the validatio'
  name: withItems
  type: array
- description: WithParam expands a task into multiple parallel tasks from the value in the parameter, which is expected to be a JSON list.
  name: withParam
  type: string
- description: WithSequence expands a task into a numeric sequence
  name: withSequence
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-dag-task-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-dag-task
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.DAGTask
---
