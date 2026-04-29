---
description: A project represents a prioritized list of tasks in Asana or a board with columns of tasks represented as cards. It exists in a single workspace or organization.
layout: schema
name: Asana Project
properties_list:
- description: Globally unique identifier of the resource.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: Name of the project.
  name: name
  type: string
- description: True if the project is archived.
  name: archived
  type: boolean
- description: Color of the project.
  name: color
  type:
  - string
  - 'null'
- description: The time at which this resource was created.
  name: created_at
  type: string
- description: The time at which this project was last modified.
  name: modified_at
  type: string
- description: The day on which this project is due (YYYY-MM-DD).
  name: due_on
  type:
  - string
  - 'null'
- description: The day on which work begins for this project (YYYY-MM-DD).
  name: start_on
  type:
  - string
  - 'null'
- description: The default view of a project.
  name: default_view
  type: string
- description: Free-form textual information associated with the project.
  name: notes
  type: string
- description: The notes of the project with formatting as HTML.
  name: html_notes
  type: string
- description: The privacy setting of the project.
  name: privacy_setting
  type: string
- description: The default access for users or teams who join the project.
  name: default_access_level
  type: string
- description: True if the project is currently marked complete.
  name: completed
  type: boolean
- description: The time at which this project was completed.
  name: completed_at
  type:
  - string
  - 'null'
- description: The current owner of the project.
  name: owner
  type: object
- description: The team that this project is shared with.
  name: team
  type: object
- description: The workspace or organization this project is associated with.
  name: workspace
  type: object
- description: Array of users who are members of this project.
  name: members
  type: array
- description: Array of users following this project.
  name: followers
  type: array
- description: The icon for a project.
  name: icon
  type:
  - string
  - 'null'
- description: A URL that points directly to the object within Asana.
  name: permalink_url
  type: string
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-project-json-schema.json
slug: asana-project-json
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.asana.com/schemas/project\",\n  \"title\": \"Asana Project\",\n  \"description\": \"A project represents a prioritized list of tasks in Asana or a board with columns of tasks represented as cards. It exists in a single workspace or organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique identifier of the resource.\",\n      \"readOnly\": true,\n      \"examples\": [\"12345\"]\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"const\": \"project\",\n      \"description\": \"The base type of this resource.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project.\",\n      \"examples\": [\"Stuff to buy\"]\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"True\
  \ if the project is archived.\"\n    },\n    \"color\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\n        \"dark-pink\", \"dark-green\", \"dark-blue\", \"dark-red\", \"dark-teal\",\n        \"dark-brown\", \"dark-orange\", \"dark-purple\", \"dark-warm-gray\",\n        \"light-pink\", \"light-green\", \"light-blue\", \"light-red\", \"light-teal\",\n        \"light-brown\", \"light-orange\", \"light-purple\", \"light-warm-gray\",\n        \"none\", null\n      ],\n      \"description\": \"Color of the project.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which this resource was created.\",\n      \"readOnly\": true\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which this project was last modified.\",\n      \"readOnly\": true\n    },\n    \"due_on\": {\n      \"type\": [\"string\", \"null\"],\n\
  \      \"format\": \"date\",\n      \"description\": \"The day on which this project is due (YYYY-MM-DD).\"\n    },\n    \"start_on\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The day on which work begins for this project (YYYY-MM-DD).\"\n    },\n    \"default_view\": {\n      \"type\": \"string\",\n      \"enum\": [\"list\", \"board\", \"calendar\", \"timeline\"],\n      \"description\": \"The default view of a project.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form textual information associated with the project.\"\n    },\n    \"html_notes\": {\n      \"type\": \"string\",\n      \"description\": \"The notes of the project with formatting as HTML.\"\n    },\n    \"privacy_setting\": {\n      \"type\": \"string\",\n      \"enum\": [\"public_to_workspace\", \"private_to_team\", \"private\"],\n      \"description\": \"The privacy setting of the project.\"\n    },\n    \"default_access_level\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"admin\", \"editor\", \"commenter\", \"viewer\"],\n      \"description\": \"The default access for users or teams who join the project.\"\n    },\n    \"completed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the project is currently marked complete.\",\n      \"readOnly\": true\n    },\n    \"completed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time at which this project was completed.\",\n      \"readOnly\": true\n    },\n    \"owner\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/UserCompact\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The current owner of the project.\"\n    },\n    \"team\": {\n      \"$ref\": \"#/$defs/TeamCompact\",\n      \"description\": \"The team that this project is shared with.\"\n    },\n    \"workspace\": {\n      \"$ref\": \"#/$defs/WorkspaceCompact\",\n      \"description\"\
  : \"The workspace or organization this project is associated with.\",\n      \"readOnly\": true\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/UserCompact\" },\n      \"description\": \"Array of users who are members of this project.\",\n      \"readOnly\": true\n    },\n    \"followers\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/UserCompact\" },\n      \"description\": \"Array of users following this project.\",\n      \"readOnly\": true\n    },\n    \"icon\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The icon for a project.\"\n    },\n    \"permalink_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL that points directly to the object within Asana.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"gid\", \"resource_type\"],\n  \"$defs\": {\n    \"UserCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n    \
  \    \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"user\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"TeamCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"team\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"WorkspaceCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"workspace\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/asana/refs/heads/main/json-schema/asana-project-json-schema.json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana Project
---
