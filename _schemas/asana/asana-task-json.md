---
description: The task is the basic object around which many operations in Asana are centered. Tasks represent units of work that can be assigned, prioritized, and tracked.
layout: schema
name: Asana Task
properties_list:
- description: Globally unique identifier of the resource, as a string.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: The subtype of this resource.
  name: resource_subtype
  type: string
- description: Name of the task. Generally a short sentence fragment.
  name: name
  type: string
- description: Conditional. Reflects the approval status of this task.
  name: approval_status
  type: string
- description: True if the task is currently marked complete.
  name: completed
  type: boolean
- description: The time at which this task was completed, or null if incomplete.
  name: completed_at
  type:
  - string
  - 'null'
- description: The user who completed this task.
  name: completed_by
  type: object
- description: The time at which this resource was created.
  name: created_at
  type: string
- description: The time at which this task was last modified.
  name: modified_at
  type: string
- description: The UTC date and time on which this task is due.
  name: due_at
  type:
  - string
  - 'null'
- description: The localized date on which this task is due (YYYY-MM-DD).
  name: due_on
  type:
  - string
  - 'null'
- description: Date and time on which work begins for the task.
  name: start_at
  type:
  - string
  - 'null'
- description: The day on which work begins for the task (YYYY-MM-DD).
  name: start_on
  type:
  - string
  - 'null'
- description: Free-form textual information associated with the task.
  name: notes
  type: string
- description: The notes of the text with formatting as HTML.
  name: html_notes
  type: string
- description: The user to whom this task is assigned.
  name: assignee
  type: object
- description: The parent of this task, or null if not a subtask.
  name: parent
  type: object
- description: Array of projects this task is associated with.
  name: projects
  type: array
- description: Array of tags associated with this task.
  name: tags
  type: array
- description: Array of users following this task.
  name: followers
  type: array
- description: The workspace this task is associated with.
  name: workspace
  type: object
- description: Array of custom field values applied to the task.
  name: custom_fields
  type: array
- description: True if the task is liked by the authorized user.
  name: liked
  type: boolean
- description: The number of users who have liked this task.
  name: num_likes
  type: integer
- description: The number of subtasks on this task.
  name: num_subtasks
  type: integer
- description: A URL that points directly to the object within Asana.
  name: permalink_url
  type: string
- description: Sum of all Time Tracking entries in the Actual Time field.
  name: actual_time_minutes
  type:
  - number
  - 'null'
- description: OAuth Required. App-specific metadata on tasks.
  name: external
  type: object
- description: Array of projects and sections this task belongs to.
  name: memberships
  type: array
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-task-json-schema.json
slug: asana-task-json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana Task
---
