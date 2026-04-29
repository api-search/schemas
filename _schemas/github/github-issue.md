---
description: A GitHub issue used for tracking bugs, feature requests, tasks, and discussions within a repository.
layout: schema
name: GitHub Issue
properties_list:
- description: The unique identifier of the issue.
  name: id
  type: integer
- description: The GraphQL node ID for the issue.
  name: node_id
  type: string
- description: The API URL for the issue.
  name: url
  type: string
- description: The URL of the issue on GitHub.
  name: html_url
  type: string
- description: The issue number within the repository.
  name: number
  type: integer
- description: The current state of the issue.
  name: state
  type: string
- description: The reason the issue state was changed.
  name: state_reason
  type:
  - string
  - 'null'
- description: The title of the issue.
  name: title
  type: string
- description: The contents of the issue in Markdown format.
  name: body
  type:
  - string
  - 'null'
- description: ''
  name: user
  type: object
- description: Labels applied to the issue.
  name: labels
  type: array
- description: The primary user assigned to the issue.
  name: assignee
  type: object
- description: All users assigned to the issue.
  name: assignees
  type: array
- description: The milestone the issue is associated with.
  name: milestone
  type: object
- description: Whether the issue is locked.
  name: locked
  type: boolean
- description: The reason the issue was locked.
  name: active_lock_reason
  type:
  - string
  - 'null'
- description: The number of comments on the issue.
  name: comments
  type: integer
- description: Pull request metadata if this issue is also a pull request.
  name: pull_request
  type: object
- description: The date and time the issue was created.
  name: created_at
  type: string
- description: The date and time the issue was last updated.
  name: updated_at
  type: string
- description: The date and time the issue was closed.
  name: closed_at
  type:
  - string
  - 'null'
- description: The user who closed the issue.
  name: closed_by
  type: object
- description: How the author is associated with the repository.
  name: author_association
  type: string
- description: ''
  name: reactions
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-issue-schema.json
slug: github-issue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/schemas/github/issue.json\",\n  \"title\": \"GitHub Issue\",\n  \"description\": \"A GitHub issue used for tracking bugs, feature requests, tasks, and discussions within a repository.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"number\", \"title\", \"state\", \"user\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the issue.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID for the issue.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the issue.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the issue on GitHub.\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"minimum\"\
  : 1,\n      \"description\": \"The issue number within the repository.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"open\", \"closed\"],\n      \"description\": \"The current state of the issue.\"\n    },\n    \"state_reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"completed\", \"reopened\", \"not_planned\", null],\n      \"description\": \"The reason the issue state was changed.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the issue.\",\n      \"minLength\": 1\n    },\n    \"body\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The contents of the issue in Markdown format.\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/SimpleUser\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the issue.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Label\"\n      }\n    },\n    \"assignee\": {\n      \"oneOf\"\
  : [\n        { \"$ref\": \"#/$defs/SimpleUser\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The primary user assigned to the issue.\"\n    },\n    \"assignees\": {\n      \"type\": \"array\",\n      \"description\": \"All users assigned to the issue.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SimpleUser\"\n      }\n    },\n    \"milestone\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/Milestone\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The milestone the issue is associated with.\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the issue is locked.\"\n    },\n    \"active_lock_reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"off-topic\", \"too heated\", \"resolved\", \"spam\", null],\n      \"description\": \"The reason the issue was locked.\"\n    },\n    \"comments\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\"\
  : \"The number of comments on the issue.\"\n    },\n    \"pull_request\": {\n      \"type\": \"object\",\n      \"description\": \"Pull request metadata if this issue is also a pull request.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for the pull request.\"\n        },\n        \"html_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the pull request on GitHub.\"\n        },\n        \"diff_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the pull request diff.\"\n        },\n        \"patch_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the pull request patch.\"\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The date and time the issue was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the issue was last updated.\"\n    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the issue was closed.\"\n    },\n    \"closed_by\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/SimpleUser\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user who closed the issue.\"\n    },\n    \"author_association\": {\n      \"type\": \"string\",\n      \"enum\": [\"COLLABORATOR\", \"CONTRIBUTOR\", \"FIRST_TIMER\", \"FIRST_TIME_CONTRIBUTOR\", \"MANNEQUIN\", \"MEMBER\", \"NONE\", \"OWNER\"],\n      \"description\": \"How the author is associated with the repository.\"\n    },\n    \"reactions\": {\n      \"$ref\": \"#/$defs/Reactions\"\n    }\n  },\n  \"$defs\": {\n    \"SimpleUser\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"A simplified representation of a GitHub user.\",\n      \"required\": [\"login\", \"id\"],\n      \"properties\": {\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for the user.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        },\n        \"avatar_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"html_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's GitHub profile.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Organization\", \"Bot\"],\n\
  \          \"description\": \"The type of account.\"\n        }\n      }\n    },\n    \"Label\": {\n      \"type\": \"object\",\n      \"description\": \"A label applied to an issue or pull request.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the label.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the label.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A description of the label.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9a-fA-F]{6}$\",\n          \"description\": \"The hex color code of the label without the # prefix.\"\n        },\n        \"\
  default\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a default label.\"\n        }\n      }\n    },\n    \"Milestone\": {\n      \"type\": \"object\",\n      \"description\": \"A milestone used to track progress on groups of issues and pull requests.\",\n      \"required\": [\"id\", \"number\", \"title\", \"state\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the milestone.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        },\n        \"number\": {\n          \"type\": \"integer\",\n          \"description\": \"The milestone number.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the milestone.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A description\
  \ of the milestone.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"open\", \"closed\"],\n          \"description\": \"The state of the milestone.\"\n        },\n        \"open_issues\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of open issues in the milestone.\"\n        },\n        \"closed_issues\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of closed issues in the milestone.\"\n        },\n        \"due_on\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The due date of the milestone.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the milestone was created.\"\n        },\n        \"closed_at\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\"\
  : \"When the milestone was closed.\"\n        }\n      }\n    },\n    \"Reactions\": {\n      \"type\": \"object\",\n      \"description\": \"Reaction counts for the issue.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for the reactions.\"\n        },\n        \"total_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total number of reactions.\"\n        },\n        \"+1\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of thumbs up reactions.\"\n        },\n        \"-1\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of thumbs down reactions.\"\n        },\n        \"laugh\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of laugh reactions.\"\n        },\n        \"hooray\"\
  : {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of hooray reactions.\"\n        },\n        \"confused\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of confused reactions.\"\n        },\n        \"heart\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of heart reactions.\"\n        },\n        \"rocket\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of rocket reactions.\"\n        },\n        \"eyes\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of eyes reactions.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-issue-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: GitHub Issue
---
