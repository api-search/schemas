---
description: A GitLab issue used for tracking work, bugs, feature requests, or incidents within a project.
layout: schema
name: GitLab Issue
properties_list:
- description: The globally unique identifier of the issue.
  name: id
  type: integer
- description: The internal project-scoped ID of the issue.
  name: iid
  type: integer
- description: The ID of the project the issue belongs to.
  name: project_id
  type: integer
- description: The title of the issue.
  name: title
  type: string
- description: The description of the issue, supporting Markdown syntax.
  name: description
  type:
  - string
  - 'null'
- description: The current state of the issue.
  name: state
  type: string
- description: The type of issue.
  name: issue_type
  type: string
- description: The GitLab-internal issue type designation.
  name: type
  type: string
- description: Labels applied to the issue.
  name: labels
  type: array
- description: The milestone the issue is associated with.
  name: milestone
  type: object
- description: ''
  name: author
  type: object
- description: Users assigned to work on this issue.
  name: assignees
  type: array
- description: The user who closed the issue.
  name: closed_by
  type: object
- description: Whether the issue is confidential and visible only to project members with Reporter access or above.
  name: confidential
  type: boolean
- description: The weight assigned to the issue for effort estimation. Requires Premium or Ultimate tier.
  name: weight
  type:
  - integer
  - 'null'
- description: The severity level of the issue. Used for incidents.
  name: severity
  type: string
- description: The number of upvotes the issue has received.
  name: upvotes
  type: integer
- description: The number of downvotes the issue has received.
  name: downvotes
  type: integer
- description: The number of user-authored comments on the issue.
  name: user_notes_count
  type: integer
- description: The number of merge requests related to this issue.
  name: merge_requests_count
  type: integer
- description: ''
  name: references
  type: object
- description: The URL to view the issue in a browser.
  name: web_url
  type: string
- description: ''
  name: time_stats
  type: object
- description: ''
  name: task_completion_status
  type: object
- description: Whether the issue description contains task list items.
  name: has_tasks
  type: boolean
- description: The due date of the issue in YYYY-MM-DD format.
  name: due_date
  type:
  - string
  - 'null'
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
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-issue-schema.json
slug: gitlab-issue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gitlab.com/schemas/gitlab/issue.json\",\n  \"title\": \"GitLab Issue\",\n  \"description\": \"A GitLab issue used for tracking work, bugs, feature requests, or incidents within a project.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"iid\", \"project_id\", \"title\", \"state\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The globally unique identifier of the issue.\"\n    },\n    \"iid\": {\n      \"type\": \"integer\",\n      \"description\": \"The internal project-scoped ID of the issue.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project the issue belongs to.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the issue.\",\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n\
  \      \"description\": \"The description of the issue, supporting Markdown syntax.\",\n      \"maxLength\": 1048576\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"opened\", \"closed\"],\n      \"description\": \"The current state of the issue.\"\n    },\n    \"issue_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"issue\", \"incident\", \"test_case\", \"task\"],\n      \"description\": \"The type of issue.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The GitLab-internal issue type designation.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the issue.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"milestone\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/Milestone\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The milestone the issue is associated with.\"\n    },\n    \"author\": {\n      \"$ref\"\
  : \"#/$defs/UserSummary\"\n    },\n    \"assignees\": {\n      \"type\": \"array\",\n      \"description\": \"Users assigned to work on this issue.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/UserSummary\"\n      }\n    },\n    \"closed_by\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/UserSummary\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user who closed the issue.\"\n    },\n    \"confidential\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the issue is confidential and visible only to project members with Reporter access or above.\"\n    },\n    \"weight\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The weight assigned to the issue for effort estimation. Requires Premium or Ultimate tier.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"UNKNOWN\", \"INFO\", \"LOW\", \"MEDIUM\", \"HIGH\", \"CRITICAL\"],\n      \"description\": \"The\
  \ severity level of the issue. Used for incidents.\"\n    },\n    \"upvotes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of upvotes the issue has received.\"\n    },\n    \"downvotes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of downvotes the issue has received.\"\n    },\n    \"user_notes_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of user-authored comments on the issue.\"\n    },\n    \"merge_requests_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of merge requests related to this issue.\"\n    },\n    \"references\": {\n      \"$ref\": \"#/$defs/References\"\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to view the issue in a browser.\"\n    },\n    \"time_stats\": {\n      \"$ref\": \"#/$defs/TimeStats\"\
  \n    },\n    \"task_completion_status\": {\n      \"$ref\": \"#/$defs/TaskCompletionStatus\"\n    },\n    \"has_tasks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the issue description contains task list items.\"\n    },\n    \"due_date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The due date of the issue in YYYY-MM-DD format.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the issue was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the issue was last updated.\"\n    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the issue was closed.\"\n    }\n  },\n  \"$defs\": {\n    \"UserSummary\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"A simplified representation of a GitLab user.\",\n      \"required\": [\"id\", \"username\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"blocked\", \"deactivated\"],\n          \"description\": \"The current state of the user account.\"\n        },\n        \"avatar_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\
  ,\n          \"description\": \"URL to the user's GitLab profile page.\"\n        }\n      }\n    },\n    \"Milestone\": {\n      \"type\": \"object\",\n      \"description\": \"A milestone that groups issues and merge requests by a target date.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the milestone.\"\n        },\n        \"iid\": {\n          \"type\": \"integer\",\n          \"description\": \"The project-scoped ID of the milestone.\"\n        },\n        \"project_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the project the milestone belongs to.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the milestone.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The description of the milestone.\"\n        },\n        \"state\":\
  \ {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"closed\"],\n          \"description\": \"The current state of the milestone.\"\n        },\n        \"due_date\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"The due date of the milestone.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to view the milestone in a browser.\"\n        }\n      }\n    },\n    \"References\": {\n      \"type\": \"object\",\n      \"description\": \"Reference strings for the issue.\",\n      \"properties\": {\n        \"short\": {\n          \"type\": \"string\",\n          \"description\": \"Short reference format, for example #42.\"\n        },\n        \"relative\": {\n          \"type\": \"string\",\n          \"description\": \"Relative reference format including project path.\"\n        },\n        \"full\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Full reference format including namespace and project path.\"\n        }\n      }\n    },\n    \"TimeStats\": {\n      \"type\": \"object\",\n      \"description\": \"Time tracking statistics for the issue.\",\n      \"properties\": {\n        \"time_estimate\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Estimated time to complete the issue in seconds.\"\n        },\n        \"total_time_spent\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total time logged against the issue in seconds.\"\n        },\n        \"human_time_estimate\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Human-readable time estimate, for example 1d 2h.\"\n        },\n        \"human_total_time_spent\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Human-readable total time spent, for example 30m.\"\n        }\n\
  \      }\n    },\n    \"TaskCompletionStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Completion status for task list items in the issue description.\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total number of task list items.\"\n        },\n        \"completed_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of completed task list items.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-issue-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: GitLab Issue
---
