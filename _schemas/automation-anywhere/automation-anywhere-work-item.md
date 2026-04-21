---
description: Schema representing a work item within the Automation Anywhere Workload Management system. A work item is a single unit of data queued for processing by an RPA bot, with a typed payload defined by the queue's work item model and lifecycle status tracking from creation through completion.
layout: schema
name: Automation Anywhere Work Item
properties_list:
- description: Unique numeric identifier of the work item assigned by the Control Room upon creation
  name: id
  type: integer
- description: Numeric ID of the Workload Management queue this work item belongs to
  name: queueId
  type: integer
- description: Key-value data payload of the work item. Keys are attribute names defined in the queue's work item model; values are the actual data to be processed by the bot.
  name: json
  type: object
- description: Current lifecycle status of the work item indicating where it is in the processing pipeline
  name: status
  type: string
- description: Processing outcome recorded by the bot upon completing or failing this work item
  name: result
  type: string
- description: 'Display column 1: a human-readable label extracted from the work item data for display in the Control Room queue viewer'
  name: col1
  type: string
- description: 'Display column 2: a secondary human-readable label extracted from the work item data'
  name: col2
  type: string
- description: 'Display column 3: a tertiary human-readable label extracted from the work item data'
  name: col3
  type: string
- description: Numeric ID of the Bot Runner device that processed or is currently processing this work item
  name: deviceId
  type: integer
- description: Numeric ID of the user account under which the processing bot executed on the device
  name: deviceUserId
  type: integer
- description: Deployment ID (UUID) of the automation that processed this work item, linking back to the deployment record
  name: automationId
  type: string
- description: Identifier of the job execution associated with processing this work item
  name: jobExecutionId
  type: string
- description: ISO 8601 timestamp when the bot began processing this work item
  name: startTime
  type: string
- description: ISO 8601 timestamp when bot processing of this work item completed
  name: endTime
  type: string
- description: ISO 8601 timestamp until which this work item is deferred; the bot will not pick it up before this time
  name: deferredUntil
  type: string
- description: ISO 8601 timestamp when the work item was last paused during processing
  name: lastPausedTime
  type: string
- description: Total time in seconds this work item was in a paused state
  name: totalPausedTime
  type: integer
- description: Optional free-text comment added by the processing bot or a human operator
  name: comment
  type: string
- description: Error message recorded when the work item processing failed, for debugging and retry decisions
  name: error
  type: string
- description: Number of times this work item has been automatically retried after failure
  name: retryCount
  type: integer
- description: Hash of the work item data used for duplicate detection when disallowDuplicate is enabled on the queue
  name: hashCode
  type: integer
- description: Optimistic concurrency control version number; must match the server value when updating
  name: version
  type: integer
- description: UUID of the tenant in a multi-tenant Control Room deployment
  name: tenantUuid
  type: string
- description: Numeric ID of the user who created this work item
  name: createdBy
  type: integer
- description: ISO 8601 timestamp when this work item was added to the queue
  name: createdOn
  type: string
- description: Numeric ID of the user who last modified this work item
  name: updatedBy
  type: integer
- description: ISO 8601 timestamp of the last status or data update to this work item
  name: updatedOn
  type: string
provider_name: automation-anywhere
provider_slug: automation-anywhere
schema_file: json-schema/automation-anywhere-work-item-schema.json
slug: automation-anywhere-work-item
tags: []
title: Automation Anywhere Work Item
---
