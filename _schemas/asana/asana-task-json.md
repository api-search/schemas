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
source_filename: asana-task-json-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.asana.com/schemas/task\",\n  \"title\": \"Asana Task\",\n  \"description\": \"The task is the basic object around which many operations in Asana are centered. Tasks represent units of work that can be assigned, prioritized, and tracked.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique identifier of the resource, as a string.\",\n      \"readOnly\": true,\n      \"examples\": [\"12345\"]\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"const\": \"task\",\n      \"description\": \"The base type of this resource.\",\n      \"readOnly\": true\n    },\n    \"resource_subtype\": {\n      \"type\": \"string\",\n      \"enum\": [\"default_task\", \"milestone\", \"section\", \"approval\"],\n      \"description\": \"The subtype of this resource.\",\n      \"examples\": [\"default_task\"\
  ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the task. Generally a short sentence fragment.\",\n      \"examples\": [\"Buy catnip\"]\n    },\n    \"approval_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"approved\", \"rejected\", \"changes_requested\"],\n      \"description\": \"Conditional. Reflects the approval status of this task.\"\n    },\n    \"completed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the task is currently marked complete.\",\n      \"examples\": [false]\n    },\n    \"completed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time at which this task was completed, or null if incomplete.\",\n      \"readOnly\": true\n    },\n    \"completed_by\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/UserCompact\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user who completed this\
  \ task.\",\n      \"readOnly\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which this resource was created.\",\n      \"readOnly\": true\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which this task was last modified.\",\n      \"readOnly\": true\n    },\n    \"due_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The UTC date and time on which this task is due.\"\n    },\n    \"due_on\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The localized date on which this task is due (YYYY-MM-DD).\"\n    },\n    \"start_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time on which work begins for the task.\"\n    },\n    \"start_on\": {\n\
  \      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The day on which work begins for the task (YYYY-MM-DD).\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form textual information associated with the task.\"\n    },\n    \"html_notes\": {\n      \"type\": \"string\",\n      \"description\": \"The notes of the text with formatting as HTML.\"\n    },\n    \"assignee\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/UserCompact\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user to whom this task is assigned.\"\n    },\n    \"parent\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/TaskCompact\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The parent of this task, or null if not a subtask.\",\n      \"readOnly\": true\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/ProjectCompact\" },\n   \
  \   \"description\": \"Array of projects this task is associated with.\",\n      \"readOnly\": true\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/TagCompact\" },\n      \"description\": \"Array of tags associated with this task.\",\n      \"readOnly\": true\n    },\n    \"followers\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/UserCompact\" },\n      \"description\": \"Array of users following this task.\",\n      \"readOnly\": true\n    },\n    \"workspace\": {\n      \"$ref\": \"#/$defs/WorkspaceCompact\",\n      \"description\": \"The workspace this task is associated with.\",\n      \"readOnly\": true\n    },\n    \"custom_fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Array of custom field values applied to the task.\",\n      \"readOnly\": true\n    },\n    \"liked\": {\n      \"type\": \"boolean\",\n      \"description\": \"True\
  \ if the task is liked by the authorized user.\"\n    },\n    \"num_likes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of users who have liked this task.\",\n      \"readOnly\": true\n    },\n    \"num_subtasks\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of subtasks on this task.\",\n      \"readOnly\": true\n    },\n    \"permalink_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL that points directly to the object within Asana.\",\n      \"readOnly\": true\n    },\n    \"actual_time_minutes\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Sum of all Time Tracking entries in the Actual Time field.\",\n      \"readOnly\": true\n    },\n    \"external\": {\n      \"type\": \"object\",\n      \"description\": \"OAuth Required. App-specific metadata on tasks.\",\n      \"properties\": {\n        \"gid\": {\n          \"type\": \"string\"\n        },\n        \"data\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"memberships\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"project\": { \"$ref\": \"#/$defs/ProjectCompact\" },\n          \"section\": { \"$ref\": \"#/$defs/SectionCompact\" }\n        }\n      },\n      \"description\": \"Array of projects and sections this task belongs to.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"gid\", \"resource_type\"],\n  \"$defs\": {\n    \"UserCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"user\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"TaskCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"task\" },\n        \"name\"\
  : { \"type\": \"string\" }\n      }\n    },\n    \"ProjectCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"project\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"TagCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"tag\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"SectionCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"section\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"WorkspaceCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\"\
  , \"const\": \"workspace\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/asana/refs/heads/main/json-schema/asana-task-json-schema.json
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
