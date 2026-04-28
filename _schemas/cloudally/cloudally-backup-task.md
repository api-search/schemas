---
description: Schema for a CloudAlly backup task. A backup task represents the configuration that protects a specific SaaS workload (Microsoft 365 mailbox, Google Workspace user, Salesforce org, Box account, or Dropbox account). The task carries identifying metadata, scheduling info, status, and links to the most recent backup snapshot.
layout: schema
name: CloudAlly Backup Task
properties_list:
- description: Unique identifier of the backup task.
  name: id
  type: string
- description: Human-readable label for the task.
  name: name
  type: string
- description: Workload type protected by the task.
  name: type
  type: string
- description: Current backup status (for example, success, failed, in_progress, paused).
  name: status
  type: string
- description: Timestamp of the most recent successful backup.
  name: lastBackup
  type:
  - string
  - 'null'
- description: Time the task was created.
  name: createdAt
  type: string
- description: Total backed-up data size in bytes for the task.
  name: size
  type:
  - integer
  - 'null'
- description: Backup schedule configuration.
  name: schedule
  type: object
provider_name: CloudAlly
provider_slug: cloudally
schema_file: json-schema/cloudally-backup-task-schema.json
slug: cloudally-backup-task
tags:
- Backup
- Box
- Data Protection
- Disaster Recovery
- Dropbox
- Google Workspace
- Microsoft 365
- OpenText
- SaaS Backup
- Salesforce
title: CloudAlly Backup Task
---
