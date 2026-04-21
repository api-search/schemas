---
description: A Task represents an asynchronous operation in VMware Cloud Foundation that tracks the progress and status of long-running infrastructure management activities.
layout: schema
name: Broadcom Task
properties_list:
- description: The unique identifier of the task.
  name: id
  type: string
- description: The name of the task.
  name: name
  type: string
- description: The type of the task operation.
  name: type
  type: string
- description: The current status of the task.
  name: status
  type: string
- description: The timestamp when the task was created.
  name: creationTimestamp
  type: string
- description: The timestamp when the task completed.
  name: completionTimestamp
  type: string
- description: Whether the task can be cancelled.
  name: isCancellable
  type: boolean
- description: Whether the task can be retried after failure.
  name: isRetryable
  type: boolean
- description: The resources associated with this task.
  name: resources
  type: array
- description: The subtasks that make up this task.
  name: subTasks
  type: array
- description: Errors encountered during task execution.
  name: errors
  type: array
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-task-schema.json
slug: broadcom-task
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Task
---
