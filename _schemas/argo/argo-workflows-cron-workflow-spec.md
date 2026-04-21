---
description: Specification of a cron workflow
layout: schema
name: CronWorkflowSpec
properties_list:
- description: Cron schedule expression
  name: schedule
  type: string
- description: Timezone for the cron schedule
  name: timezone
  type: string
- description: ''
  name: startingDeadlineSeconds
  type: integer
- description: ''
  name: concurrencyPolicy
  type: string
- description: Whether the cron workflow is suspended
  name: suspend
  type: boolean
- description: ''
  name: successfulJobsHistoryLimit
  type: integer
- description: ''
  name: failedJobsHistoryLimit
  type: integer
- description: ''
  name: workflowSpec
  type: object
- description: ''
  name: workflowMetadata
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-cron-workflow-spec-schema.json
slug: argo-workflows-cron-workflow-spec
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: CronWorkflowSpec
---
