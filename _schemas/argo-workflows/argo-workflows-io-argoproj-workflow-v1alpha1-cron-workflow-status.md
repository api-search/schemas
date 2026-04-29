---
description: CronWorkflowStatus is the status of a CronWorkflow
layout: schema
name: io.argoproj.workflow.v1alpha1.CronWorkflowStatus
properties_list:
- description: Active is a list of active workflows stemming from this CronWorkflow
  name: active
  type: array
- description: Conditions is a list of conditions the CronWorkflow may have
  name: conditions
  type: array
- description: 'v3.6 and after: Failed counts how many times child workflows failed'
  name: failed
  type: integer
- description: LastScheduleTime is the last time the CronWorkflow was scheduled
  name: lastScheduledTime
  type: object
- description: 'v3.6 and after: Phase is an enum of Active or Stopped. It changes to Stopped when stopStrategy.expression is true'
  name: phase
  type: string
- description: 'v3.6 and after: Succeeded counts how many times child workflows succeeded'
  name: succeeded
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.CronWorkflowStatus\",\n  \"description\": \"CronWorkflowStatus is the status of a CronWorkflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"description\": \"Active is a list of active workflows stemming from this CronWorkflow\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.ObjectReference\"\n      }\n    },\n    \"conditions\": {\n      \"description\": \"Conditions is a list of conditions the CronWorkflow may have\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Condition\"\n      }\n    },\n    \"failed\": {\n      \"description\"\
  : \"v3.6 and after: Failed counts how many times child workflows failed\",\n      \"type\": \"integer\"\n    },\n    \"lastScheduledTime\": {\n      \"description\": \"LastScheduleTime is the last time the CronWorkflow was scheduled\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"phase\": {\n      \"description\": \"v3.6 and after: Phase is an enum of Active or Stopped. It changes to Stopped when stopStrategy.expression is true\",\n      \"type\": \"string\"\n    },\n    \"succeeded\": {\n      \"description\": \"v3.6 and after: Succeeded counts how many times child workflows succeeded\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-cron-workflow-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.CronWorkflowStatus
---
