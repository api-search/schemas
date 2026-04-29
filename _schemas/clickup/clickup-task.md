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
source_filename: clickup-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.clickup.com/schemas/clickup/task.json\",\n  \"title\": \"ClickUp Task\",\n  \"description\": \"A task object representing a unit of work in ClickUp. Tasks are the core entity in ClickUp and contain information about assignees, status, priority, due dates, custom fields, time tracking, and more.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the task.\"\n    },\n    \"custom_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The custom task ID if enabled for the Workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task.\",\n      \"minLength\": 1\n    },\n    \"text_content\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The plain\
  \ text content of the task description.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The task description in rich text format.\"\n    },\n    \"markdown_description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The task description in Markdown format.\"\n    },\n    \"status\": {\n      \"$ref\": \"#/$defs/Status\"\n    },\n    \"orderindex\": {\n      \"type\": \"string\",\n      \"description\": \"The order index of the task within its list.\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"description\": \"Unix timestamp in milliseconds when the task was created.\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"date_updated\": {\n      \"type\": \"string\",\n      \"description\": \"Unix timestamp in milliseconds when the task was last updated.\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"date_closed\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"\
  Unix timestamp in milliseconds when the task was closed.\"\n    },\n    \"date_done\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unix timestamp in milliseconds when the task was marked done.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task is archived.\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"assignees\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/User\"\n      },\n      \"description\": \"The users assigned to the task.\"\n    },\n    \"watchers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/User\"\n      },\n      \"description\": \"The users watching the task.\"\n    },\n    \"checklists\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Checklist\"\n      },\n      \"description\": \"Checklists attached to the task.\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"description\": \"Tags applied to the task.\"\n    },\n    \"parent\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the parent task if this is a subtask.\"\n    },\n    \"priority\": {\n      \"$ref\": \"#/$defs/Priority\"\n    },\n    \"due_date\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unix timestamp in milliseconds for the due date.\"\n    },\n    \"start_date\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unix timestamp in milliseconds for the start date.\"\n    },\n    \"points\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Sprint points assigned to the task.\",\n      \"minimum\": 0\n    },\n    \"time_estimate\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Time estimate in milliseconds.\",\n      \"minimum\": 0\n    },\n    \"time_spent\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Total time tracked on the task in milliseconds.\",\n      \"minimum\": 0\n    },\n    \"custom_fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomFieldValue\"\n      },\n      \"description\": \"Custom field values set on the task.\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Dependency\"\n      },\n      \"description\": \"Task dependencies.\"\n    },\n    \"linked_tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LinkedTask\"\n      },\n      \"description\": \"Tasks linked to this task.\"\n    },\n    \"team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workspace ID the task belongs to.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the task in the ClickUp web application.\"\n    },\n    \"list\": {\n      \"$ref\":\
  \ \"#/$defs/ListReference\"\n    },\n    \"project\": {\n      \"$ref\": \"#/$defs/FolderReference\"\n    },\n    \"folder\": {\n      \"$ref\": \"#/$defs/FolderReference\"\n    },\n    \"space\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The space ID.\"\n        }\n      },\n      \"description\": \"The space the task belongs to.\"\n    }\n  },\n  \"$defs\": {\n    \"Status\": {\n      \"type\": \"object\",\n      \"description\": \"A task status indicating the current state of work.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The status ID.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status name.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The hex color code of the status.\",\n          \"pattern\": \"^#[0-9a-fA-F]{6}$\"\
  \n        },\n        \"orderindex\": {\n          \"type\": \"integer\",\n          \"description\": \"The order index of the status.\",\n          \"minimum\": 0\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"open\", \"custom\", \"closed\", \"done\"],\n          \"description\": \"The status type category.\"\n        }\n      },\n      \"required\": [\"status\", \"type\"]\n    },\n    \"User\": {\n      \"type\": \"object\",\n      \"description\": \"A ClickUp user.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the user.\"\n        },\n        \"color\": {\n    \
  \      \"type\": \"string\",\n          \"description\": \"The hex color code associated with the user.\"\n        },\n        \"profilePicture\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL of the user's profile picture.\"\n        },\n        \"initials\": {\n          \"type\": \"string\",\n          \"description\": \"The initials of the user.\",\n          \"maxLength\": 3\n        }\n      },\n      \"required\": [\"id\", \"username\"]\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A tag applied to a task.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the tag.\"\n        },\n        \"tag_fg\": {\n          \"type\": \"string\",\n          \"description\": \"Foreground color of the tag.\"\n        },\n        \"tag_bg\": {\n          \"type\": \"string\",\n          \"description\": \"Background color of\
  \ the tag.\"\n        },\n        \"creator\": {\n          \"type\": \"integer\",\n          \"description\": \"The user ID of the tag creator.\"\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"Priority\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Task priority level.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The priority ID.\"\n        },\n        \"priority\": {\n          \"type\": \"string\",\n          \"enum\": [\"urgent\", \"high\", \"normal\", \"low\"],\n          \"description\": \"The priority level name.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The hex color code of the priority level.\"\n        },\n        \"orderindex\": {\n          \"type\": \"string\",\n          \"description\": \"The order index of the priority.\"\n        }\n      }\n    },\n    \"CustomFieldValue\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A custom field value on a task.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The custom field ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The custom field name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"url\", \"drop_down\", \"email\", \"phone\", \"date\", \"text\",\n            \"checkbox\", \"number\", \"currency\", \"tasks\", \"users\",\n            \"emoji\", \"label\", \"automatic_progress\", \"manual_progress\",\n            \"short_text\", \"location\"\n          ],\n          \"description\": \"The type of the custom field.\"\n        },\n        \"type_config\": {\n          \"type\": \"object\",\n          \"description\": \"Configuration specific to the custom field type.\"\n        },\n        \"date_created\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Unix timestamp when the custom field was created.\"\n        },\n        \"hide_from_guests\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the field is hidden from guests.\"\n        },\n        \"value\": {\n          \"description\": \"The current value of the custom field. Type varies by field type.\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the custom field is required.\"\n        }\n      },\n      \"required\": [\"id\", \"name\", \"type\"]\n    },\n    \"Checklist\": {\n      \"type\": \"object\",\n      \"description\": \"A checklist attached to a task.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The checklist ID.\"\n        },\n        \"task_id\": {\n          \"type\": \"string\",\n          \"description\": \"The task ID the checklist belongs to.\"\n        },\n        \"name\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The name of the checklist.\"\n        },\n        \"orderindex\": {\n          \"type\": \"integer\",\n          \"description\": \"The order index.\"\n        },\n        \"resolved\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of resolved items.\",\n          \"minimum\": 0\n        },\n        \"unresolved\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of unresolved items.\",\n          \"minimum\": 0\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The checklist item ID.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The item text.\"\n              },\n              \"orderindex\": {\n                \"type\": \"integer\"\
  ,\n                \"description\": \"The order index.\"\n              },\n              \"assignee\": {\n                \"type\": [\"object\", \"null\"],\n                \"description\": \"The assigned user.\"\n              },\n              \"resolved\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the item is resolved.\"\n              },\n              \"parent\": {\n                \"type\": [\"string\", \"null\"],\n                \"description\": \"The parent checklist item ID for nested items.\"\n              },\n              \"date_created\": {\n                \"type\": \"string\",\n                \"description\": \"Unix timestamp when created.\"\n              },\n              \"children\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\"\n                },\n                \"description\": \"Nested checklist items.\"\n              }\n            }\n          },\n\
  \          \"description\": \"The items in the checklist.\"\n        }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"Dependency\": {\n      \"type\": \"object\",\n      \"description\": \"A dependency between two tasks.\",\n      \"properties\": {\n        \"task_id\": {\n          \"type\": \"string\",\n          \"description\": \"The dependent task ID.\"\n        },\n        \"depends_on\": {\n          \"type\": \"string\",\n          \"description\": \"The task ID this task depends on.\"\n        },\n        \"type\": {\n          \"type\": \"integer\",\n          \"description\": \"The dependency type code.\"\n        },\n        \"date_created\": {\n          \"type\": \"string\",\n          \"description\": \"Unix timestamp when the dependency was created.\"\n        },\n        \"userid\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID who created the dependency.\"\n        }\n      }\n    },\n    \"LinkedTask\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"A task linked to another task.\",\n      \"properties\": {\n        \"task_id\": {\n          \"type\": \"string\",\n          \"description\": \"The linked task ID.\"\n        },\n        \"link_id\": {\n          \"type\": \"string\",\n          \"description\": \"The link ID.\"\n        },\n        \"date_created\": {\n          \"type\": \"string\",\n          \"description\": \"Unix timestamp when the link was created.\"\n        },\n        \"userid\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID who created the link.\"\n        }\n      }\n    },\n    \"ListReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a list.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The list ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The list name.\"\n        },\n        \"access\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has access to the list.\"\n        }\n      }\n    },\n    \"FolderReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a folder.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The folder ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The folder name.\"\n        },\n        \"access\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has access to the folder.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/json-schema/clickup-task-schema.json
tags: []
title: ClickUp Task
---
