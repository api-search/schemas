---
description: An asynchronous task
layout: schema
name: Task
properties_list:
- description: Unique task identifier
  name: taskId
  type: string
- description: Task type
  name: type
  type: string
- description: Task status
  name: status
  type: string
- description: When the task was submitted
  name: submitDate
  type: string
- description: When the task started executing
  name: startedDate
  type: string
- description: When the task completed
  name: completedDate
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-task-schema.json
slug: webadmin-rest-api-task
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: Task
---
