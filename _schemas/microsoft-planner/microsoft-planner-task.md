---
description: Represents a Planner task in Microsoft 365 as defined by the Microsoft Graph API v1.0. A task is contained in a plannerPlan and can be assigned to a plannerBucket within the plan. Each task can be assigned to users, categorized, and tracked for completion.
layout: schema
name: Microsoft Planner Task
properties_list:
- description: The ETag of the resource, used for optimistic concurrency control via the If-Match header on PATCH and DELETE operations.
  name: '@odata.etag'
  type: string
- description: Read-only unique identifier of the task. It is 28 characters long and case-sensitive. Format validation is performed by the service.
  name: id
  type: string
- description: Title of the task.
  name: title
  type: string
- description: The ID of the plan to which the task belongs. Tasks cannot be created without specifying a plan.
  name: planId
  type: string
- description: The ID of the bucket to which the task belongs. The bucket must be in the same plan as the task. It is 28 characters long and case-sensitive.
  name: bucketId
  type:
  - string
  - 'null'
- description: The set of assignees the task is assigned to. Each key is the user ID of the assignee.
  name: assignments
  type: object
- description: The categories (labels) applied to the task. Category names are defined on the plan details.
  name: appliedCategories
  type: object
- description: Priority of the task. Valid range is 0-10, with 0 being highest priority. Values 0-1 map to 'urgent', 2-4 to 'important', 5-7 to 'medium', and 8-10 to 'low'. Planner sets 1 for urgent, 3 for important
  name: priority
  type: integer
- description: Percentage of task completion. When set to 100, the task is considered completed.
  name: percentComplete
  type: integer
- description: Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
  name: startDateTime
  type:
  - string
  - 'null'
- description: Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
  name: dueDateTime
  type:
  - string
  - 'null'
- description: Read-only. Date and time at which the percentComplete of the task was set to 100. ISO 8601 format, always in UTC.
  name: completedDateTime
  type:
  - string
  - 'null'
- description: Read-only. Identity of the user that completed the task.
  name: completedBy
  type: object
- description: Read-only. Date and time at which the task was created. ISO 8601 format, always in UTC.
  name: createdDateTime
  type: string
- description: Read-only. Identity of the user that created the task.
  name: createdBy
  type: object
- description: Read-only. True if the details object of the task has a nonempty description, false otherwise.
  name: hasDescription
  type: boolean
- description: Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.
  name: conversationThreadId
  type:
  - string
  - 'null'
- description: Hint used to order items of this type in a list view. The format is defined by the Planner order hints specification.
  name: orderHint
  type: string
- description: Hint used to order items of this type in a list view when grouped by the user assigned to.
  name: assigneePriority
  type: string
- description: The type of preview that shows up on the task.
  name: previewType
  type: string
- description: Read-only. Number of checklist items with value set to false, representing incomplete items.
  name: activeChecklistItemCount
  type: integer
- description: Read-only. Total number of checklist items present on the task.
  name: checklistItemCount
  type: integer
- description: Read-only. Number of external references that exist on the task.
  name: referenceCount
  type: integer
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-task-schema.json
slug: microsoft-planner-task
source_filename: microsoft-planner-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.example.com/microsoft-planner/task\",\n  \"title\": \"Microsoft Planner Task\",\n  \"description\": \"Represents a Planner task in Microsoft 365 as defined by the Microsoft Graph API v1.0. A task is contained in a plannerPlan and can be assigned to a plannerBucket within the plan. Each task can be assigned to users, categorized, and tracked for completion.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"planId\",\n    \"title\"\n  ],\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the resource, used for optimistic concurrency control via the If-Match header on PATCH and DELETE operations.\",\n      \"readOnly\": true\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Read-only unique identifier of the task. It is 28 characters long and case-sensitive. Format validation is performed by\
  \ the service.\",\n      \"readOnly\": true,\n      \"minLength\": 28,\n      \"maxLength\": 28\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the task.\",\n      \"minLength\": 1\n    },\n    \"planId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the plan to which the task belongs. Tasks cannot be created without specifying a plan.\",\n      \"minLength\": 28,\n      \"maxLength\": 28\n    },\n    \"bucketId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the bucket to which the task belongs. The bucket must be in the same plan as the task. It is 28 characters long and case-sensitive.\",\n      \"minLength\": 28,\n      \"maxLength\": 28\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the task.\"\n    },\n    \"assignments\": {\n      \"$ref\": \"#/$defs/plannerAssignments\",\n      \"description\": \"The set of assignees the task is assigned to.\
  \ Each key is the user ID of the assignee.\"\n    },\n    \"appliedCategories\": {\n      \"$ref\": \"#/$defs/plannerAppliedCategories\",\n      \"description\": \"The categories (labels) applied to the task. Category names are defined on the plan details.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the task. Valid range is 0-10, with 0 being highest priority. Values 0-1 map to 'urgent', 2-4 to 'important', 5-7 to 'medium', and 8-10 to 'low'. Planner sets 1 for urgent, 3 for important, 5 for medium, and 9 for low.\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n      \"default\": 5\n    },\n    \"percentComplete\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of task completion. When set to 100, the task is considered completed.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"default\": 0\n    },\n    \"startDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.\"\n    },\n    \"dueDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.\"\n    },\n    \"completedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Read-only. Date and time at which the percentComplete of the task was set to 100. ISO 8601 format, always in UTC.\",\n      \"readOnly\": true\n    },\n    \"completedBy\": {\n      \"$ref\": \"#/$defs/identitySet\",\n      \"description\": \"Read-only. Identity of the user that completed the task.\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Read-only. Date and time at which the task was created. ISO 8601 format, always in UTC.\",\n      \"readOnly\": true\n    },\n    \"createdBy\": {\n      \"$ref\": \"#/$defs/identitySet\",\n      \"description\": \"Read-only. Identity of the user that created the task.\",\n      \"readOnly\": true\n    },\n    \"hasDescription\": {\n      \"type\": \"boolean\",\n      \"description\": \"Read-only. True if the details object of the task has a nonempty description, false otherwise.\",\n      \"readOnly\": true\n    },\n    \"conversationThreadId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order items of this type in a list view. The format is defined by the Planner order hints specification.\"\n    },\n    \"\
  assigneePriority\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order items of this type in a list view when grouped by the user assigned to.\"\n    },\n    \"previewType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of preview that shows up on the task.\",\n      \"enum\": [\n        \"automatic\",\n        \"noPreview\",\n        \"checklist\",\n        \"description\",\n        \"reference\"\n      ],\n      \"default\": \"automatic\"\n    },\n    \"activeChecklistItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Read-only. Number of checklist items with value set to false, representing incomplete items.\",\n      \"readOnly\": true,\n      \"minimum\": 0\n    },\n    \"checklistItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Read-only. Total number of checklist items present on the task.\",\n      \"readOnly\": true,\n      \"minimum\": 0\n    },\n    \"referenceCount\": {\n      \"type\":\
  \ \"integer\",\n      \"description\": \"Read-only. Number of external references that exist on the task.\",\n      \"readOnly\": true,\n      \"minimum\": 0\n    }\n  },\n  \"$defs\": {\n    \"identitySet\": {\n      \"type\": \"object\",\n      \"description\": \"A set of identities associated with various events for a resource, such as created by or last modified by.\",\n      \"properties\": {\n        \"application\": {\n          \"$ref\": \"#/$defs/identity\"\n        },\n        \"device\": {\n          \"$ref\": \"#/$defs/identity\"\n        },\n        \"user\": {\n          \"$ref\": \"#/$defs/identity\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"identity\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an identity of an actor (user, application, or device).\",\n      \"properties\": {\n        \"displayName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The display name of the identity.\"\
  \n        },\n        \"id\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The unique identifier of the identity.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"plannerAssignments\": {\n      \"type\": \"object\",\n      \"description\": \"The set of user assignments for a task. Each property name (key) is the user ID of the assignee, and the value is a plannerAssignment object.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/plannerAssignment\"\n      }\n    },\n    \"plannerAssignment\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the assignment of a task to a user.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"const\": \"microsoft.graph.plannerAssignment\"\n        },\n        \"assignedBy\": {\n          \"$ref\": \"#/$defs/identitySet\",\n          \"description\": \"The identity of the user that performed the assignment of\
  \ the task.\",\n          \"readOnly\": true\n        },\n        \"assignedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time at which the task was assigned. ISO 8601 format, always in UTC.\",\n          \"readOnly\": true\n        },\n        \"orderHint\": {\n          \"type\": \"string\",\n          \"description\": \"Hint used to order assignees in a task.\"\n        }\n      },\n      \"required\": [\n        \"@odata.type\",\n        \"orderHint\"\n      ],\n      \"additionalProperties\": false\n    },\n    \"plannerAppliedCategories\": {\n      \"type\": \"object\",\n      \"description\": \"The categories (labels) applied to a task. Up to 25 categories can be defined per plan. Each property name is a category identifier (category1 through category25) and the value is a boolean indicating whether the category is applied.\",\n      \"properties\": {\n        \"category1\": { \"type\": \"boolean\" },\n   \
  \     \"category2\": { \"type\": \"boolean\" },\n        \"category3\": { \"type\": \"boolean\" },\n        \"category4\": { \"type\": \"boolean\" },\n        \"category5\": { \"type\": \"boolean\" },\n        \"category6\": { \"type\": \"boolean\" },\n        \"category7\": { \"type\": \"boolean\" },\n        \"category8\": { \"type\": \"boolean\" },\n        \"category9\": { \"type\": \"boolean\" },\n        \"category10\": { \"type\": \"boolean\" },\n        \"category11\": { \"type\": \"boolean\" },\n        \"category12\": { \"type\": \"boolean\" },\n        \"category13\": { \"type\": \"boolean\" },\n        \"category14\": { \"type\": \"boolean\" },\n        \"category15\": { \"type\": \"boolean\" },\n        \"category16\": { \"type\": \"boolean\" },\n        \"category17\": { \"type\": \"boolean\" },\n        \"category18\": { \"type\": \"boolean\" },\n        \"category19\": { \"type\": \"boolean\" },\n        \"category20\": { \"type\": \"boolean\" },\n        \"category21\"\
  : { \"type\": \"boolean\" },\n        \"category22\": { \"type\": \"boolean\" },\n        \"category23\": { \"type\": \"boolean\" },\n        \"category24\": { \"type\": \"boolean\" },\n        \"category25\": { \"type\": \"boolean\" }\n      },\n      \"additionalProperties\": false\n    },\n    \"plannerTaskDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the additional information about a task, retrieved via the /details relationship. Includes description, checklist items, and external references.\",\n      \"properties\": {\n        \"@odata.etag\": {\n          \"type\": \"string\",\n          \"description\": \"The ETag of the resource.\",\n          \"readOnly\": true\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Read-only. The unique identifier for the task details. 28 characters long and case-sensitive.\",\n          \"readOnly\": true\n        },\n        \"description\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Description of the task.\"\n        },\n        \"checklist\": {\n          \"$ref\": \"#/$defs/plannerChecklistItems\",\n          \"description\": \"The collection of checklist items on the task.\"\n        },\n        \"references\": {\n          \"$ref\": \"#/$defs/plannerExternalReferences\",\n          \"description\": \"The collection of external references on the task.\"\n        },\n        \"previewType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of preview that shows up on the task. When set to automatic, the displayed preview is chosen by the app viewing the task.\",\n          \"enum\": [\n            \"automatic\",\n            \"noPreview\",\n            \"checklist\",\n            \"description\",\n            \"reference\"\n          ]\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"plannerChecklistItems\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of\
  \ checklist items on a task. Each key is a GUID identifying the checklist item.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/plannerChecklistItem\"\n      }\n    },\n    \"plannerChecklistItem\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a single checklist item on a Planner task.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"const\": \"microsoft.graph.plannerChecklistItem\"\n        },\n        \"isChecked\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the checklist item is checked (completed).\",\n          \"default\": false\n        },\n        \"lastModifiedBy\": {\n          \"$ref\": \"#/$defs/identitySet\",\n          \"description\": \"Identity of the user that last modified the checklist item.\",\n          \"readOnly\": true\n        },\n        \"lastModifiedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n\
  \          \"description\": \"The date and time the item was last modified. ISO 8601 format, always in UTC.\",\n          \"readOnly\": true\n        },\n        \"orderHint\": {\n          \"type\": \"string\",\n          \"description\": \"Hint used to order items in the checklist.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Title of the checklist item.\"\n        }\n      },\n      \"required\": [\"title\"],\n      \"additionalProperties\": false\n    },\n    \"plannerExternalReferences\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of external references on a task. Each key is a URL-encoded URL of the reference.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/plannerExternalReference\"\n      }\n    },\n    \"plannerExternalReference\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an external reference (link or file) attached to a Planner task.\",\n      \"properties\"\
  : {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"const\": \"microsoft.graph.plannerExternalReference\"\n        },\n        \"alias\": {\n          \"type\": \"string\",\n          \"description\": \"A name alias to describe the reference.\"\n        },\n        \"lastModifiedBy\": {\n          \"$ref\": \"#/$defs/identitySet\",\n          \"description\": \"Identity of the user that last modified the reference.\",\n          \"readOnly\": true\n        },\n        \"lastModifiedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the reference was last modified. ISO 8601 format, always in UTC.\",\n          \"readOnly\": true\n        },\n        \"previewPriority\": {\n          \"type\": \"string\",\n          \"description\": \"Hint used to set the relative priority order in which the reference will be shown as a preview on the task.\"\n        },\n        \"type\": {\n    \
  \      \"type\": \"string\",\n          \"description\": \"The type of the reference, used to represent the type of resource (e.g., PowerPoint, Word, Excel, Other).\"\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": \"ABCDEFGHIJKLMNOPQRSTUVWXYZab\",\n      \"title\": \"Review project requirements\",\n      \"planId\": \"ABCDEFGHIJKLMNOPQRSTUVWXYZab\",\n      \"bucketId\": \"ABCDEFGHIJKLMNOPQRSTUVWXYZab\",\n      \"assignments\": {\n        \"user-id-1\": {\n          \"@odata.type\": \"microsoft.graph.plannerAssignment\",\n          \"orderHint\": \"8586352891559904378\"\n        }\n      },\n      \"appliedCategories\": {\n        \"category1\": true,\n        \"category3\": true\n      },\n      \"priority\": 3,\n      \"percentComplete\": 50,\n      \"startDateTime\": \"2026-03-01T09:00:00Z\",\n      \"dueDateTime\": \"2026-03-15T17:00:00Z\",\n      \"completedDateTime\": null,\n    \
  \  \"createdDateTime\": \"2026-02-28T12:00:00Z\",\n      \"hasDescription\": true,\n      \"previewType\": \"automatic\",\n      \"activeChecklistItemCount\": 2,\n      \"checklistItemCount\": 5,\n      \"referenceCount\": 1\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-task-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: Microsoft Planner Task
---
