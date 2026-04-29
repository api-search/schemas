---
description: A GitHub pull request representing a proposed change to a repository, including metadata for code review, merging, and CI/CD status.
layout: schema
name: GitHub Pull Request
properties_list:
- description: The unique identifier of the pull request.
  name: id
  type: integer
- description: The GraphQL node ID for the pull request.
  name: node_id
  type: string
- description: The API URL for the pull request.
  name: url
  type: string
- description: The URL of the pull request on GitHub.
  name: html_url
  type: string
- description: The URL to the pull request diff.
  name: diff_url
  type: string
- description: The URL to the pull request patch.
  name: patch_url
  type: string
- description: The pull request number within the repository.
  name: number
  type: integer
- description: The current state of the pull request.
  name: state
  type: string
- description: Whether the pull request is locked.
  name: locked
  type: boolean
- description: The title of the pull request.
  name: title
  type: string
- description: The contents of the pull request description in Markdown format.
  name: body
  type:
  - string
  - 'null'
- description: ''
  name: user
  type: object
- description: Labels applied to the pull request.
  name: labels
  type: array
- description: Users assigned to the pull request.
  name: assignees
  type: array
- description: Users requested to review the pull request.
  name: requested_reviewers
  type: array
- description: Teams requested to review the pull request.
  name: requested_teams
  type: array
- description: ''
  name: head
  type: object
- description: ''
  name: base
  type: object
- description: Whether the pull request is a draft.
  name: draft
  type: boolean
- description: Whether the pull request has been merged.
  name: merged
  type: boolean
- description: Whether the pull request can be merged. Null if not yet computed.
  name: mergeable
  type:
  - boolean
  - 'null'
- description: The mergeability state of the pull request.
  name: mergeable_state
  type: string
- description: The SHA of the merge commit, if merged.
  name: merge_commit_sha
  type:
  - string
  - 'null'
- description: The user who merged the pull request.
  name: merged_by
  type: object
- description: The number of comments on the pull request.
  name: comments
  type: integer
- description: The number of review comments on the pull request.
  name: review_comments
  type: integer
- description: The number of commits in the pull request.
  name: commits
  type: integer
- description: The number of lines added.
  name: additions
  type: integer
- description: The number of lines deleted.
  name: deletions
  type: integer
- description: The number of changed files.
  name: changed_files
  type: integer
- description: The date and time the pull request was created.
  name: created_at
  type: string
- description: The date and time the pull request was last updated.
  name: updated_at
  type: string
- description: The date and time the pull request was closed.
  name: closed_at
  type:
  - string
  - 'null'
- description: The date and time the pull request was merged.
  name: merged_at
  type:
  - string
  - 'null'
- description: Auto-merge configuration if enabled.
  name: auto_merge
  type:
  - object
  - 'null'
- description: How the author is associated with the repository.
  name: author_association
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-pull-request-schema.json
slug: github-pull-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/schemas/github/pull-request.json\",\n  \"title\": \"GitHub Pull Request\",\n  \"description\": \"A GitHub pull request representing a proposed change to a repository, including metadata for code review, merging, and CI/CD status.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"number\", \"title\", \"state\", \"user\", \"head\", \"base\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the pull request.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID for the pull request.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the pull request.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the pull\
  \ request on GitHub.\"\n    },\n    \"diff_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the pull request diff.\"\n    },\n    \"patch_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the pull request patch.\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The pull request number within the repository.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"open\", \"closed\"],\n      \"description\": \"The current state of the pull request.\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the pull request is locked.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the pull request.\",\n      \"minLength\": 1\n    },\n    \"body\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The contents\
  \ of the pull request description in Markdown format.\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/SimpleUser\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the pull request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Label\"\n      }\n    },\n    \"assignees\": {\n      \"type\": \"array\",\n      \"description\": \"Users assigned to the pull request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SimpleUser\"\n      }\n    },\n    \"requested_reviewers\": {\n      \"type\": \"array\",\n      \"description\": \"Users requested to review the pull request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SimpleUser\"\n      }\n    },\n    \"requested_teams\": {\n      \"type\": \"array\",\n      \"description\": \"Teams requested to review the pull request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Team\"\n      }\n    },\n    \"head\": {\n      \"$ref\": \"#/$defs/BranchRef\"\n    },\n    \"base\"\
  : {\n      \"$ref\": \"#/$defs/BranchRef\"\n    },\n    \"draft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the pull request is a draft.\"\n    },\n    \"merged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the pull request has been merged.\"\n    },\n    \"mergeable\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the pull request can be merged. Null if not yet computed.\"\n    },\n    \"mergeable_state\": {\n      \"type\": \"string\",\n      \"description\": \"The mergeability state of the pull request.\"\n    },\n    \"merge_commit_sha\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The SHA of the merge commit, if merged.\"\n    },\n    \"merged_by\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/SimpleUser\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user who merged the pull request.\"\n    },\n    \"comments\": {\n      \"type\": \"integer\"\
  ,\n      \"minimum\": 0,\n      \"description\": \"The number of comments on the pull request.\"\n    },\n    \"review_comments\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of review comments on the pull request.\"\n    },\n    \"commits\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of commits in the pull request.\"\n    },\n    \"additions\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of lines added.\"\n    },\n    \"deletions\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of lines deleted.\"\n    },\n    \"changed_files\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of changed files.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pull request was created.\"\
  \n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pull request was last updated.\"\n    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pull request was closed.\"\n    },\n    \"merged_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pull request was merged.\"\n    },\n    \"auto_merge\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Auto-merge configuration if enabled.\",\n      \"properties\": {\n        \"enabled_by\": {\n          \"$ref\": \"#/$defs/SimpleUser\"\n        },\n        \"merge_method\": {\n          \"type\": \"string\",\n          \"enum\": [\"merge\", \"squash\", \"rebase\"],\n          \"description\": \"The merge method to use.\"\n        },\n        \"commit_title\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The commit title for the auto-merge.\"\n        },\n        \"commit_message\": {\n          \"type\": \"string\",\n          \"description\": \"The commit message for the auto-merge.\"\n        }\n      }\n    },\n    \"author_association\": {\n      \"type\": \"string\",\n      \"enum\": [\"COLLABORATOR\", \"CONTRIBUTOR\", \"FIRST_TIMER\", \"FIRST_TIME_CONTRIBUTOR\", \"MANNEQUIN\", \"MEMBER\", \"NONE\", \"OWNER\"],\n      \"description\": \"How the author is associated with the repository.\"\n    }\n  },\n  \"$defs\": {\n    \"SimpleUser\": {\n      \"type\": \"object\",\n      \"description\": \"A simplified representation of a GitHub user.\",\n      \"required\": [\"login\", \"id\"],\n      \"properties\": {\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique\
  \ identifier for the user.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        },\n        \"avatar_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"html_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's GitHub profile.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Organization\", \"Bot\"],\n          \"description\": \"The type of account.\"\n        }\n      }\n    },\n    \"Label\": {\n      \"type\": \"object\",\n      \"description\": \"A label applied to an issue or pull request.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the label.\"\
  \n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the label.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9a-fA-F]{6}$\",\n          \"description\": \"The hex color code of the label.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A description of the label.\"\n        }\n      }\n    },\n    \"Team\": {\n      \"type\": \"object\",\n      \"description\": \"A GitHub team within an organization.\",\n      \"required\": [\"id\", \"name\", \"slug\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the team.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"\
  The name of the team.\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"The URL-friendly slug of the team name.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A description of the team.\"\n        },\n        \"privacy\": {\n          \"type\": \"string\",\n          \"enum\": [\"closed\", \"secret\"],\n          \"description\": \"The privacy level of the team.\"\n        },\n        \"permission\": {\n          \"type\": \"string\",\n          \"description\": \"The default permission level for repositories.\"\n        }\n      }\n    },\n    \"BranchRef\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a branch in a repository.\",\n      \"required\": [\"label\", \"ref\", \"sha\"],\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"The label for the branch in owner:branch format.\"\n\
  \        },\n        \"ref\": {\n          \"type\": \"string\",\n          \"description\": \"The branch name.\"\n        },\n        \"sha\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9a-f]{40}$\",\n          \"description\": \"The SHA of the head commit on the branch.\"\n        },\n        \"user\": {\n          \"$ref\": \"#/$defs/SimpleUser\"\n        },\n        \"repo\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The repository the branch belongs to.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\",\n              \"description\": \"The repository ID.\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The repository name.\"\n            },\n            \"full_name\": {\n              \"type\": \"string\",\n              \"description\": \"The full repository name.\"\n            },\n            \"owner\": {\n        \
  \      \"$ref\": \"#/$defs/SimpleUser\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-pull-request-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: GitHub Pull Request
---
