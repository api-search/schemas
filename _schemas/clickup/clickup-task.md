---
description: A task object representing a unit of work in ClickUp. Tasks are the core entity in ClickUp and contain information about assignees, status, priority, due dates, custom fields, time tracking, and more.
layout: schema
name: ClickUp Task
properties_list:
- description: The unique identifier of the task.
  name: id
  type: string
- description: The custom task ID if enabled for the Workspace.
  name: custom_id
  type:
  - string
  - 'null'
- description: The name of the task.
  name: name
  type: string
- description: The plain text content of the task description.
  name: text_content
  type:
  - string
  - 'null'
- description: The task description in rich text format.
  name: description
  type:
  - string
  - 'null'
- description: The task description in Markdown format.
  name: markdown_description
  type:
  - string
  - 'null'
- description: ''
  name: status
  type: object
- description: The order index of the task within its list.
  name: orderindex
  type: string
- description: Unix timestamp in milliseconds when the task was created.
  name: date_created
  type: string
- description: Unix timestamp in milliseconds when the task was last updated.
  name: date_updated
  type: string
- description: Unix timestamp in milliseconds when the task was closed.
  name: date_closed
  type:
  - string
  - 'null'
- description: Unix timestamp in milliseconds when the task was marked done.
  name: date_done
  type:
  - string
  - 'null'
- description: Whether the task is archived.
  name: archived
  type: boolean
- description: ''
  name: creator
  type: object
- description: The users assigned to the task.
  name: assignees
  type: array
- description: The users watching the task.
  name: watchers
  type: array
- description: Checklists attached to the task.
  name: checklists
  type: array
- description: Tags applied to the task.
  name: tags
  type: array
- description: The ID of the parent task if this is a subtask.
  name: parent
  type:
  - string
  - 'null'
- description: ''
  name: priority
  type: object
- description: Unix timestamp in milliseconds for the due date.
  name: due_date
  type:
  - string
  - 'null'
- description: Unix timestamp in milliseconds for the start date.
  name: start_date
  type:
  - string
  - 'null'
- description: Sprint points assigned to the task.
  name: points
  type:
  - number
  - 'null'
- description: Time estimate in milliseconds.
  name: time_estimate
  type:
  - integer
  - 'null'
- description: Total time tracked on the task in milliseconds.
  name: time_spent
  type: integer
- description: Custom field values set on the task.
  name: custom_fields
  type: array
- description: Task dependencies.
  name: dependencies
  type: array
- description: Tasks linked to this task.
  name: linked_tasks
  type: array
- description: The Workspace ID the task belongs to.
  name: team_id
  type: string
- description: The URL to the task in the ClickUp web application.
  name: url
  type: string
- description: ''
  name: list
  type: object
- description: ''
  name: project
  type: object
- description: ''
  name: folder
  type: object
- description: The space the task belongs to.
  name: space
  type: object
provider_name: clickup
provider_slug: clickup
schema_file: json-schema/clickup-task-schema.json
slug: clickup-task
tags: []
title: ClickUp Task
---
