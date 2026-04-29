---
description: A Jira project used to organize and track issues. Projects can be software, service desk, or business type and may be team-managed (next-gen) or company-managed (classic).
layout: schema
name: Jira Project
properties_list:
- description: The URL of the project in the Jira REST API.
  name: self
  type: string
- description: The unique identifier of the project.
  name: id
  type: string
- description: The project key used as a prefix for issue keys (e.g., PROJ).
  name: key
  type: string
- description: The name of the project.
  name: name
  type: string
- description: A description of the project.
  name: description
  type:
  - string
  - 'null'
- description: A URL associated with the project.
  name: url
  type:
  - string
  - 'null'
- description: ''
  name: lead
  type: object
- description: The type of the project.
  name: projectTypeKey
  type: string
- description: Whether the project uses simplified (team-managed/next-gen) configuration.
  name: simplified
  type: boolean
- description: The project style indicating its management model.
  name: style
  type: string
- description: Whether the project is archived.
  name: archived
  type: boolean
- description: Whether the project is in the trash.
  name: deleted
  type: boolean
- description: The default assignee type when creating issues in this project.
  name: assigneeType
  type: string
- description: The components defined in the project.
  name: components
  type: array
- description: The issue types available in the project.
  name: issueTypes
  type: array
- description: The versions (releases) defined in the project.
  name: versions
  type: array
- description: A mapping of role names to their REST API URLs.
  name: roles
  type: object
- description: ''
  name: avatarUrls
  type: object
- description: ''
  name: projectCategory
  type: object
- description: ''
  name: insight
  type: object
- description: ''
  name: permissions
  type: object
- description: Entity properties stored on the project.
  name: properties
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-project-schema.json
slug: jira-project
source_filename: jira-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.atlassian.com/schemas/jira/project.json\",\n  \"title\": \"Jira Project\",\n  \"description\": \"A Jira project used to organize and track issues. Projects can be software, service desk, or business type and may be team-managed (next-gen) or company-managed (classic).\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"key\", \"name\"],\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the project in the Jira REST API.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the project.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The project key used as a prefix for issue keys (e.g., PROJ).\",\n      \"pattern\": \"^[A-Z][A-Z0-9_]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The name of the project.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A description of the project.\"\n    },\n    \"url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"A URL associated with the project.\"\n    },\n    \"lead\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"projectTypeKey\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the project.\",\n      \"enum\": [\"software\", \"service_desk\", \"business\"]\n    },\n    \"simplified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project uses simplified (team-managed/next-gen) configuration.\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"The project style indicating its management model.\",\n      \"enum\": [\"classic\", \"next-gen\"]\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the project is archived.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is in the trash.\"\n    },\n    \"assigneeType\": {\n      \"type\": \"string\",\n      \"description\": \"The default assignee type when creating issues in this project.\",\n      \"enum\": [\"PROJECT_LEAD\", \"UNASSIGNED\"]\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"description\": \"The components defined in the project.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Component\"\n      }\n    },\n    \"issueTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The issue types available in the project.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/IssueType\"\n      }\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"The versions (releases) defined in the project.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Version\"\n      }\n    },\n    \"roles\": {\n    \
  \  \"type\": \"object\",\n      \"description\": \"A mapping of role names to their REST API URLs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"avatarUrls\": {\n      \"$ref\": \"#/$defs/AvatarUrls\"\n    },\n    \"projectCategory\": {\n      \"$ref\": \"#/$defs/ProjectCategory\"\n    },\n    \"insight\": {\n      \"$ref\": \"#/$defs/ProjectInsight\"\n    },\n    \"permissions\": {\n      \"$ref\": \"#/$defs/ProjectPermissions\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Entity properties stored on the project.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"$defs\": {\n    \"User\": {\n      \"type\": \"object\",\n      \"description\": \"A Jira Cloud user.\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The unique account ID for the user across all Atlassian products.\",\n          \"maxLength\": 128\n        },\n        \"emailAddress\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user account is active.\"\n        },\n        \"timeZone\": {\n          \"type\": \"string\"\n        },\n        \"accountType\": {\n          \"type\": \"string\",\n          \"enum\": [\"atlassian\", \"app\", \"customer\"]\n        },\n        \"avatarUrls\": {\n          \"$ref\": \"#/$defs/AvatarUrls\"\n        }\n      }\n    },\n    \"Component\": {\n      \"type\": \"object\",\n      \"description\": \"A project component used to group issues within a project.\",\n      \"properties\": {\n        \"self\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"uri\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the component.\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A description of the component.\"\n        },\n        \"lead\": {\n          \"$ref\": \"#/$defs/User\"\n        },\n        \"assigneeType\": {\n          \"type\": \"string\",\n          \"description\": \"The default assignee type for issues in this component.\",\n          \"enum\": [\"PROJECT_DEFAULT\", \"COMPONENT_LEAD\", \"PROJECT_LEAD\", \"UNASSIGNED\"]\n        },\n        \"assignee\": {\n          \"$ref\": \"#/$defs/User\"\n        },\n        \"realAssigneeType\": {\n          \"type\": \"string\",\n          \"description\": \"The actual assignee type used after resolution of fallbacks.\",\n          \"enum\": [\"PROJECT_DEFAULT\"\
  , \"COMPONENT_LEAD\", \"PROJECT_LEAD\", \"UNASSIGNED\"]\n        },\n        \"realAssignee\": {\n          \"$ref\": \"#/$defs/User\"\n        },\n        \"project\": {\n          \"type\": \"string\",\n          \"description\": \"The project key.\"\n        },\n        \"projectId\": {\n          \"type\": \"integer\",\n          \"description\": \"The project ID.\"\n        },\n        \"isAssigneeTypeValid\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"IssueType\": {\n      \"type\": \"object\",\n      \"description\": \"An issue type available in the project.\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the issue type (e.g., Bug, Story, Task, Epic, Sub-task).\"\n        },\n        \"description\": {\n          \"type\"\
  : \"string\"\n        },\n        \"iconUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"subtask\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this issue type is used to create sub-tasks.\"\n        },\n        \"avatarId\": {\n          \"type\": \"integer\"\n        },\n        \"hierarchyLevel\": {\n          \"type\": \"integer\",\n          \"description\": \"The hierarchy level of the issue type.\"\n        },\n        \"scope\": {\n          \"$ref\": \"#/$defs/Scope\"\n        }\n      }\n    },\n    \"Version\": {\n      \"type\": \"object\",\n      \"description\": \"A project version (release).\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the version.\"\n        },\n\
  \        \"description\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"archived\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the version is archived.\"\n        },\n        \"released\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the version has been released.\"\n        },\n        \"releaseDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The release date in YYYY-MM-DD format.\"\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The start date in YYYY-MM-DD format.\"\n        },\n        \"overdue\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the version is overdue.\"\n        },\n        \"projectId\": {\n          \"type\": \"integer\"\n        },\n        \"userReleaseDate\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The release date in the user's locale format.\"\n        },\n        \"userStartDate\": {\n          \"type\": \"string\",\n          \"description\": \"The start date in the user's locale format.\"\n        }\n      }\n    },\n    \"ProjectCategory\": {\n      \"type\": \"object\",\n      \"description\": \"A category for organizing projects.\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the project category.\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"ProjectInsight\": {\n      \"type\": \"object\",\n      \"description\": \"Insight data about the project.\",\n      \"properties\": {\n        \"totalIssueCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The\
  \ total number of issues in the project.\"\n        },\n        \"lastIssueUpdateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the most recent issue was updated.\"\n        }\n      }\n    },\n    \"ProjectPermissions\": {\n      \"type\": \"object\",\n      \"description\": \"The permissions the current user has for this project.\",\n      \"properties\": {\n        \"canEdit\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can edit the project.\"\n        }\n      }\n    },\n    \"Scope\": {\n      \"type\": \"object\",\n      \"description\": \"The scope of an issue type.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"PROJECT\", \"TEMPLATE\"]\n        },\n        \"project\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\"\n        \
  \    },\n            \"key\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"AvatarUrls\": {\n      \"type\": \"object\",\n      \"description\": \"Avatar image URLs in multiple sizes.\",\n      \"properties\": {\n        \"16x16\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"24x24\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"32x32\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"48x48\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-project-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Jira Project
---
