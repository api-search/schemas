---
description: A Linear issue representing a unit of work within a team
layout: schema
name: Linear Issue
properties_list:
- description: Unique UUID identifier for the issue
  name: id
  type: string
- description: Human-readable identifier like ENG-123
  name: identifier
  type: string
- description: Title of the issue
  name: title
  type: string
- description: Markdown description of the issue
  name: description
  type: string
- description: 'Priority: 0=No Priority, 1=Urgent, 2=High, 3=Medium, 4=Low'
  name: priority
  type: integer
- description: Story point estimate
  name: estimate
  type: number
- description: ''
  name: state
  type: object
- description: ''
  name: assignee
  type: object
- description: ''
  name: creator
  type: object
- description: ''
  name: team
  type: object
- description: ''
  name: project
  type: object
- description: ''
  name: cycle
  type: object
- description: ''
  name: labels
  type: array
- description: Direct URL to the issue in Linear
  name: url
  type: string
- description: Suggested git branch name for the issue
  name: branchName
  type: string
- description: Due date for the issue
  name: dueDate
  type: string
- description: Timestamp when the issue was completed
  name: completedAt
  type:
  - string
  - 'null'
- description: Timestamp when the issue was canceled
  name: canceledAt
  type:
  - string
  - 'null'
- description: Timestamp when work on the issue started
  name: startedAt
  type:
  - string
  - 'null'
- description: Timestamp when the issue was created
  name: createdAt
  type: string
- description: Timestamp when the issue was last updated
  name: updatedAt
  type: string
- description: Sequential number within the team
  name: number
  type: integer
- description: Whether the issue is in the trash
  name: trashed
  type: boolean
provider_name: linear
provider_slug: linear
schema_file: json-schema/linear-issue-schema.json
slug: linear-issue
source_filename: linear-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/json-schema/linear-issue-schema.json\",\n  \"title\": \"Linear Issue\",\n  \"description\": \"A Linear issue representing a unit of work within a team\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique UUID identifier for the issue\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable identifier like ENG-123\",\n      \"pattern\": \"^[A-Z]+-[0-9]+$\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the issue\",\n      \"minLength\": 1,\n      \"maxLength\": 512\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Markdown description of the issue\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Priority: 0=No Priority, 1=Urgent, 2=High, 3=Medium, 4=Low\",\n      \"enum\": [0, 1, 2, 3, 4]\n    },\n    \"estimate\": {\n      \"type\": \"number\",\n      \"description\": \"Story point estimate\"\n    },\n    \"state\": {\n      \"$ref\": \"#/$defs/WorkflowState\"\n    },\n    \"assignee\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"team\": {\n      \"$ref\": \"#/$defs/Team\"\n    },\n    \"project\": {\n      \"$ref\": \"#/$defs/Project\"\n    },\n    \"cycle\": {\n      \"$ref\": \"#/$defs/Cycle\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/IssueLabel\"\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Direct URL to the issue in Linear\"\n    },\n    \"branchName\": {\n      \"type\": \"string\",\n      \"description\": \"Suggested git branch name for the issue\"\n    },\n    \"dueDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Due date for the issue\"\n    },\n    \"completedAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the issue was completed\"\n    },\n    \"canceledAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the issue was canceled\"\n    },\n    \"startedAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when work on the issue started\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the issue was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the issue was last updated\"\n    },\n    \"number\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"Sequential number within the team\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the issue is in the trash\"\n    }\n  },\n  \"required\": [\"id\", \"identifier\", \"title\", \"createdAt\", \"updatedAt\"],\n  \"$defs\": {\n    \"WorkflowState\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow state of an issue\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"triage\", \"backlog\", \"unstarted\", \"started\", \"completed\", \"cancelled\"]\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"Hex color code\",\n          \"pattern\": \"^#[0-9a-fA-F]{6}$\"\n        }\n      },\n      \"required\": [\"id\", \"name\", \"type\"]\n    },\n    \"User\": {\n      \"type\": \"object\",\n      \"description\": \"\
  A Linear user\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"email\": { \"type\": \"string\", \"format\": \"email\" },\n        \"displayName\": { \"type\": \"string\" },\n        \"avatarUrl\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"active\": { \"type\": \"boolean\" }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"Team\": {\n      \"type\": \"object\",\n      \"description\": \"A Linear team\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Short team identifier used in issue identifiers\"\n        },\n        \"description\": { \"type\": \"string\" }\n      },\n      \"required\": [\"id\", \"name\", \"key\"]\n    },\n    \"Project\": {\n      \"type\": \"object\",\n      \"description\": \"A Linear project grouping related\
  \ issues\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"planned\", \"started\", \"paused\", \"completed\", \"cancelled\"]\n        },\n        \"progress\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Completion progress from 0 to 1\"\n        }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"Cycle\": {\n      \"type\": \"object\",\n      \"description\": \"A sprint cycle in Linear\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"number\": { \"type\": \"integer\" },\n        \"name\": { \"type\": \"string\" },\n        \"startsAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"endsAt\": { \"type\": \"string\", \"format\": \"date-time\" }\n      },\n\
  \      \"required\": [\"id\", \"number\"]\n    },\n    \"IssueLabel\": {\n      \"type\": \"object\",\n      \"description\": \"A label applied to an issue\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"color\": { \"type\": \"string\", \"pattern\": \"^#[0-9a-fA-F]{6}$\" }\n      },\n      \"required\": [\"id\", \"name\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/json-schema/linear-issue-schema.json
tags: []
title: Linear Issue
---
