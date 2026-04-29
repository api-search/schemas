---
description: A GitLab merge request proposing changes from a source branch to be merged into a target branch within a project.
layout: schema
name: GitLab Merge Request
properties_list:
- description: The globally unique identifier of the merge request.
  name: id
  type: integer
- description: The internal project-scoped ID of the merge request.
  name: iid
  type: integer
- description: The ID of the project the merge request belongs to.
  name: project_id
  type: integer
- description: The title of the merge request.
  name: title
  type: string
- description: The description of the merge request, supporting Markdown syntax.
  name: description
  type:
  - string
  - 'null'
- description: The current state of the merge request.
  name: state
  type: string
- description: Whether the merge request is in draft state and not ready for review.
  name: draft
  type: boolean
- description: The name of the source branch containing the changes.
  name: source_branch
  type: string
- description: The name of the target branch to merge changes into.
  name: target_branch
  type: string
- description: The ID of the project containing the source branch.
  name: source_project_id
  type: integer
- description: The ID of the project containing the target branch.
  name: target_project_id
  type: integer
- description: ''
  name: author
  type: object
- description: Users assigned to review and merge this merge request.
  name: assignees
  type: array
- description: Users requested to review this merge request.
  name: reviewers
  type: array
- description: The user who merged the merge request.
  name: merge_user
  type: object
- description: Labels applied to the merge request.
  name: labels
  type: array
- description: The milestone the merge request is associated with.
  name: milestone
  type: object
- description: The detailed merge readiness status of the merge request.
  name: detailed_merge_status
  type: string
- description: The HEAD commit SHA of the source branch.
  name: sha
  type:
  - string
  - 'null'
- description: The SHA of the merge commit, set after merging.
  name: merge_commit_sha
  type:
  - string
  - 'null'
- description: The SHA of the squash commit, set after squash merging.
  name: squash_commit_sha
  type:
  - string
  - 'null'
- description: Whether the merge request is configured to squash commits on merge.
  name: squash
  type: boolean
- description: ''
  name: references
  type: object
- description: The URL to view the merge request in a browser.
  name: web_url
  type: string
- description: The number of upvotes the merge request has received.
  name: upvotes
  type: integer
- description: The number of downvotes the merge request has received.
  name: downvotes
  type: integer
- description: The number of user-authored comments on the merge request.
  name: user_notes_count
  type: integer
- description: The number of files changed. May be a string for large diffs.
  name: changes_count
  type:
  - string
  - 'null'
- description: The date and time the merge request was created.
  name: created_at
  type: string
- description: The date and time the merge request was last updated.
  name: updated_at
  type: string
- description: The date and time the merge request was merged.
  name: merged_at
  type:
  - string
  - 'null'
- description: The date and time the merge request was prepared for merging.
  name: prepared_at
  type:
  - string
  - 'null'
- description: The date and time the merge request was closed without merging.
  name: closed_at
  type:
  - string
  - 'null'
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-merge-request-schema.json
slug: gitlab-merge-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gitlab.com/schemas/gitlab/merge-request.json\",\n  \"title\": \"GitLab Merge Request\",\n  \"description\": \"A GitLab merge request proposing changes from a source branch to be merged into a target branch within a project.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"iid\", \"project_id\", \"title\", \"state\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The globally unique identifier of the merge request.\"\n    },\n    \"iid\": {\n      \"type\": \"integer\",\n      \"description\": \"The internal project-scoped ID of the merge request.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project the merge request belongs to.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the merge request.\",\n      \"maxLength\": 255\n    },\n\
  \    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The description of the merge request, supporting Markdown syntax.\",\n      \"maxLength\": 1048576\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"opened\", \"closed\", \"merged\", \"locked\"],\n      \"description\": \"The current state of the merge request.\"\n    },\n    \"draft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the merge request is in draft state and not ready for review.\"\n    },\n    \"source_branch\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the source branch containing the changes.\"\n    },\n    \"target_branch\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the target branch to merge changes into.\"\n    },\n    \"source_project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project containing the source branch.\"\n    },\n    \"target_project_id\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project containing the target branch.\"\n    },\n    \"author\": {\n      \"$ref\": \"#/$defs/UserSummary\"\n    },\n    \"assignees\": {\n      \"type\": \"array\",\n      \"description\": \"Users assigned to review and merge this merge request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/UserSummary\"\n      }\n    },\n    \"reviewers\": {\n      \"type\": \"array\",\n      \"description\": \"Users requested to review this merge request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/UserSummary\"\n      }\n    },\n    \"merge_user\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/UserSummary\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user who merged the merge request.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the merge request.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n \
  \   \"milestone\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/Milestone\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The milestone the merge request is associated with.\"\n    },\n    \"detailed_merge_status\": {\n      \"type\": \"string\",\n      \"description\": \"The detailed merge readiness status of the merge request.\",\n      \"enum\": [\n        \"blocked_status\",\n        \"broken_status\",\n        \"checking\",\n        \"ci_must_pass\",\n        \"ci_still_running\",\n        \"discussions_not_resolved\",\n        \"draft_status\",\n        \"external_status_checks\",\n        \"mergeable\",\n        \"not_approved\",\n        \"not_open\",\n        \"policies_denied\",\n        \"unchecked\"\n      ]\n    },\n    \"sha\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The HEAD commit SHA of the source branch.\"\n    },\n    \"merge_commit_sha\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\":\
  \ \"The SHA of the merge commit, set after merging.\"\n    },\n    \"squash_commit_sha\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The SHA of the squash commit, set after squash merging.\"\n    },\n    \"squash\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the merge request is configured to squash commits on merge.\"\n    },\n    \"references\": {\n      \"$ref\": \"#/$defs/References\"\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to view the merge request in a browser.\"\n    },\n    \"upvotes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of upvotes the merge request has received.\"\n    },\n    \"downvotes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of downvotes the merge request has received.\"\n    },\n    \"user_notes_count\": {\n      \"type\": \"integer\",\n\
  \      \"minimum\": 0,\n      \"description\": \"The number of user-authored comments on the merge request.\"\n    },\n    \"changes_count\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The number of files changed. May be a string for large diffs.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the merge request was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the merge request was last updated.\"\n    },\n    \"merged_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the merge request was merged.\"\n    },\n    \"prepared_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the merge request was prepared for merging.\"\n\
  \    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the merge request was closed without merging.\"\n    }\n  },\n  \"$defs\": {\n    \"UserSummary\": {\n      \"type\": \"object\",\n      \"description\": \"A simplified representation of a GitLab user.\",\n      \"required\": [\"id\", \"username\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"blocked\", \"deactivated\"],\n          \"description\": \"The current state of the user account.\"\
  \n        },\n        \"avatar_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's GitLab profile page.\"\n        }\n      }\n    },\n    \"Milestone\": {\n      \"type\": \"object\",\n      \"description\": \"A milestone that groups issues and merge requests by a target date.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the milestone.\"\n        },\n        \"iid\": {\n          \"type\": \"integer\",\n          \"description\": \"The project-scoped ID of the milestone.\"\n        },\n        \"project_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the project the milestone belongs to.\"\n        },\n        \"title\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The title of the milestone.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The description of the milestone.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"closed\"],\n          \"description\": \"The current state of the milestone.\"\n        },\n        \"due_date\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"The due date of the milestone in YYYY-MM-DD format.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to view the milestone in a browser.\"\n        }\n      }\n    },\n    \"References\": {\n      \"type\": \"object\",\n      \"description\": \"Reference strings for the merge request.\",\n      \"properties\": {\n        \"short\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Short reference format, for example !42.\"\n        },\n        \"relative\": {\n          \"type\": \"string\",\n          \"description\": \"Relative reference format including project path.\"\n        },\n        \"full\": {\n          \"type\": \"string\",\n          \"description\": \"Full reference format including namespace and project path.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-merge-request-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: GitLab Merge Request
---
