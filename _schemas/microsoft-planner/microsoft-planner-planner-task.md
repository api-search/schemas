---
description: Represents a Planner task in Microsoft 365. A task is contained in a plan and can be assigned to a bucket within the plan.
layout: schema
name: PlannerTask
properties_list:
- description: The ETag of the resource, used for concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier for the task. 28 characters long and case-sensitive.
  name: id
  type: string
- description: Title of the task
  name: title
  type: string
- description: Plan ID to which the task belongs
  name: planId
  type: string
- description: Bucket ID to which the task belongs. The bucket must be in the same plan as the task. 28 characters long and case-sensitive.
  name: bucketId
  type: '[''string'', ''null'']'
- description: Priority of the task. Valid range is 0-10 where 0 is highest priority. Values 0-1 are urgent, 2-4 are important, 5-7 are medium, 8-10 are low.
  name: priority
  type: integer
- description: Percentage of task completion. When set to 100, the task is considered completed.
  name: percentComplete
  type: integer
- description: Date and time at which the task starts. ISO 8601 format, always in UTC.
  name: startDateTime
  type: '[''string'', ''null'']'
- description: Date and time at which the task is due. ISO 8601 format, always in UTC.
  name: dueDateTime
  type: '[''string'', ''null'']'
- description: Date and time at which the percentComplete was set to 100. ISO 8601 format, always in UTC.
  name: completedDateTime
  type: '[''string'', ''null'']'
- description: Date and time at which the task was created. ISO 8601 format, always in UTC.
  name: createdDateTime
  type: string
- description: Indicates whether the details object of the task has a nonempty description.
  name: hasDescription
  type: boolean
- description: Thread ID of the conversation on the task in the containing group.
  name: conversationThreadId
  type: '[''string'', ''null'']'
- description: Hint used to order items of this type in a list view
  name: orderHint
  type: string
- description: Hint used to order items of this type when grouped by assignee
  name: assigneePriority
  type: string
- description: The type of preview that shows on the task
  name: previewType
  type: string
- description: Number of incomplete checklist items
  name: activeChecklistItemCount
  type: integer
- description: Total number of checklist items on the task
  name: checklistItemCount
  type: integer
- description: Number of external references on the task
  name: referenceCount
  type: integer
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-task-schema.json
slug: microsoft-planner-planner-task
source_filename: microsoft-planner-planner-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerTask\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Planner task in Microsoft 365. A task is contained in a plan and can be assigned to a bucket within the plan.\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the resource, used for concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the task. 28 characters long and case-sensitive.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the task\"\n    },\n    \"planId\": {\n      \"type\": \"string\",\n      \"description\": \"Plan ID to which the task belongs\"\n    },\n    \"bucketId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Bucket ID to which the task belongs. The bucket must be in the same plan as the task. 28\
  \ characters long and case-sensitive.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the task. Valid range is 0-10 where 0 is highest priority. Values 0-1 are urgent, 2-4 are important, 5-7 are medium, 8-10 are low.\"\n    },\n    \"percentComplete\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of task completion. When set to 100, the task is considered completed.\"\n    },\n    \"startDateTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date and time at which the task starts. ISO 8601 format, always in UTC.\"\n    },\n    \"dueDateTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date and time at which the task is due. ISO 8601 format, always in UTC.\"\n    },\n    \"completedDateTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date and time at which the percentComplete was set to 100. ISO 8601 format, always in UTC.\"\n    },\n\
  \    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time at which the task was created. ISO 8601 format, always in UTC.\"\n    },\n    \"hasDescription\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the details object of the task has a nonempty description.\"\n    },\n    \"conversationThreadId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Thread ID of the conversation on the task in the containing group.\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order items of this type in a list view\"\n    },\n    \"assigneePriority\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order items of this type when grouped by assignee\"\n    },\n    \"previewType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of preview that shows on the task\"\n    },\n    \"activeChecklistItemCount\": {\n      \"type\":\
  \ \"integer\",\n      \"description\": \"Number of incomplete checklist items\"\n    },\n    \"checklistItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of checklist items on the task\"\n    },\n    \"referenceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of external references on the task\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-task-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerTask
---
