---
description: CronWorkflowSpec is the specification of a CronWorkflow
layout: schema
name: io.argoproj.workflow.v1alpha1.CronWorkflowSpec
properties_list:
- description: ConcurrencyPolicy is the K8s-style concurrency policy that will be used
  name: concurrencyPolicy
  type: string
- description: FailedJobsHistoryLimit is the number of failed jobs to be kept at a time
  name: failedJobsHistoryLimit
  type: integer
- description: 'v3.6 and after: Schedules is a list of schedules to run the Workflow in Cron format'
  name: schedules
  type: array
- description: StartingDeadlineSeconds is the K8s-style deadline that will limit the time a CronWorkflow will be run after its original scheduled time if it is missed.
  name: startingDeadlineSeconds
  type: integer
- description: 'v3.6 and after: StopStrategy defines if the CronWorkflow should stop scheduling based on a condition'
  name: stopStrategy
  type: object
- description: SuccessfulJobsHistoryLimit is the number of successful jobs to be kept at a time
  name: successfulJobsHistoryLimit
  type: integer
- description: Suspend is a flag that will stop new CronWorkflows from running if set to true
  name: suspend
  type: boolean
- description: Timezone is the timezone against which the cron schedule will be calculated, e.g. "Asia/Tokyo". Default is machine's local time.
  name: timezone
  type: string
- description: 'v3.6 and after: When is an expression that determines if a run should be scheduled.'
  name: when
  type: string
- description: WorkflowMetadata contains some metadata of the workflow to be run
  name: workflowMetadata
  type: object
- description: WorkflowSpec is the spec of the workflow to be run
  name: workflowSpec
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-spec-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-spec-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.CronWorkflowSpec\",\n  \"description\": \"CronWorkflowSpec is the specification of a CronWorkflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"concurrencyPolicy\": {\n      \"description\": \"ConcurrencyPolicy is the K8s-style concurrency policy that will be used\",\n      \"type\": \"string\"\n    },\n    \"failedJobsHistoryLimit\": {\n      \"description\": \"FailedJobsHistoryLimit is the number of failed jobs to be kept at a time\",\n      \"type\": \"integer\"\n    },\n    \"schedules\": {\n      \"description\": \"v3.6 and after: Schedules is a list of schedules to run the Workflow in Cron format\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\"\
  : \"string\"\n      }\n    },\n    \"startingDeadlineSeconds\": {\n      \"description\": \"StartingDeadlineSeconds is the K8s-style deadline that will limit the time a CronWorkflow will be run after its original scheduled time if it is missed.\",\n      \"type\": \"integer\"\n    },\n    \"stopStrategy\": {\n      \"description\": \"v3.6 and after: StopStrategy defines if the CronWorkflow should stop scheduling based on a condition\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.StopStrategy\"\n    },\n    \"successfulJobsHistoryLimit\": {\n      \"description\": \"SuccessfulJobsHistoryLimit is the number of successful jobs to be kept at a time\",\n      \"type\": \"integer\"\n    },\n    \"suspend\": {\n      \"description\": \"Suspend is a flag that will stop new CronWorkflows from running if set to true\",\n      \"type\": \"boolean\"\n    },\n    \"timezone\": {\n      \"description\": \"Timezone is the timezone against which the cron schedule will be calculated,\
  \ e.g. \\\"Asia/Tokyo\\\". Default is machine's local time.\",\n      \"type\": \"string\"\n    },\n    \"when\": {\n      \"description\": \"v3.6 and after: When is an expression that determines if a run should be scheduled.\",\n      \"type\": \"string\"\n    },\n    \"workflowMetadata\": {\n      \"description\": \"WorkflowMetadata contains some metadata of the workflow to be run\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta\"\n    },\n    \"workflowSpec\": {\n      \"description\": \"WorkflowSpec is the spec of the workflow to be run\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowSpec\"\n    }\n  },\n  \"required\": [\n    \"workflowSpec\",\n    \"schedules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-spec-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.CronWorkflowSpec
---
