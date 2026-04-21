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
