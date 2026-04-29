---
description: A GitLab project containing a Git repository, issues, merge requests, CI/CD pipelines, and other DevOps resources.
layout: schema
name: GitLab Project
properties_list:
- description: The unique identifier of the project.
  name: id
  type: integer
- description: The display name of the project.
  name: name
  type: string
- description: A short description of the project.
  name: description
  type:
  - string
  - 'null'
- description: The URL-friendly path component of the project name.
  name: path
  type: string
- description: The full path of the project including the namespace, such as group/project-name.
  name: path_with_namespace
  type: string
- description: The full name of the project including the namespace.
  name: name_with_namespace
  type: string
- description: The visibility level of the project.
  name: visibility
  type: string
- description: The URL to access the project in a browser.
  name: web_url
  type: string
- description: The HTTP URL for cloning the repository.
  name: http_url_to_repo
  type: string
- description: The SSH URL for cloning the repository.
  name: ssh_url_to_repo
  type: string
- description: The URL to the README file of the default branch.
  name: readme_url
  type:
  - string
  - 'null'
- description: The default branch of the repository.
  name: default_branch
  type:
  - string
  - 'null'
- description: List of topic tags associated with the project.
  name: topics
  type: array
- description: Whether the project is archived and read-only.
  name: archived
  type: boolean
- description: Whether the repository has been initialized with commits.
  name: empty_repo
  type: boolean
- description: ''
  name: namespace
  type: object
- description: ''
  name: owner
  type: object
- description: The ID of the user who created the project.
  name: creator_id
  type: integer
- description: The number of stars the project has received.
  name: star_count
  type: integer
- description: The number of forks of the project.
  name: forks_count
  type: integer
- description: The number of open issues in the project.
  name: open_issues_count
  type: integer
- description: The path to the CI/CD configuration file relative to the repository root.
  name: ci_config_path
  type:
  - string
  - 'null'
- description: The access level for the issues feature.
  name: issues_access_level
  type: string
- description: The access level for the merge requests feature.
  name: merge_requests_access_level
  type: string
- description: The access level for CI/CD pipelines and builds.
  name: builds_access_level
  type: string
- description: The access level for the project wiki.
  name: wiki_access_level
  type: string
- description: The access level for the container registry.
  name: container_registry_access_level
  type: string
- description: The access level for GitLab Pages.
  name: pages_access_level
  type: string
- description: ''
  name: permissions
  type: object
- description: ''
  name: statistics
  type: object
- description: The date and time the project was created.
  name: created_at
  type: string
- description: The date and time the project was last updated.
  name: updated_at
  type: string
- description: The date and time of the last activity in the project.
  name: last_activity_at
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-project-schema.json
slug: gitlab-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gitlab.com/schemas/gitlab/project.json\",\n  \"title\": \"GitLab Project\",\n  \"description\": \"A GitLab project containing a Git repository, issues, merge requests, CI/CD pipelines, and other DevOps resources.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"path\", \"path_with_namespace\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the project.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A short description of the project.\",\n      \"maxLength\": 2000\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly path component of the project name.\",\n      \"pattern\": \"^[a-zA-Z0-9_.-]+$\"\
  \n    },\n    \"path_with_namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The full path of the project including the namespace, such as group/project-name.\"\n    },\n    \"name_with_namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the project including the namespace.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"private\", \"internal\", \"public\"],\n      \"description\": \"The visibility level of the project.\"\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to access the project in a browser.\"\n    },\n    \"http_url_to_repo\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The HTTP URL for cloning the repository.\"\n    },\n    \"ssh_url_to_repo\": {\n      \"type\": \"string\",\n      \"description\": \"The SSH URL for cloning the repository.\"\n    },\n    \"readme_url\": {\n\
  \      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URL to the README file of the default branch.\"\n    },\n    \"default_branch\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The default branch of the repository.\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"List of topic tags associated with the project.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is archived and read-only.\"\n    },\n    \"empty_repo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository has been initialized with commits.\"\n    },\n    \"namespace\": {\n      \"$ref\": \"#/$defs/Namespace\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/$defs/UserSummary\"\n    },\n    \"creator_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user\
  \ who created the project.\"\n    },\n    \"star_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of stars the project has received.\"\n    },\n    \"forks_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of forks of the project.\"\n    },\n    \"open_issues_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of open issues in the project.\"\n    },\n    \"ci_config_path\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The path to the CI/CD configuration file relative to the repository root.\",\n      \"default\": \".gitlab-ci.yml\"\n    },\n    \"issues_access_level\": {\n      \"type\": \"string\",\n      \"enum\": [\"disabled\", \"private\", \"enabled\", \"public\"],\n      \"description\": \"The access level for the issues feature.\"\n    },\n    \"merge_requests_access_level\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\"disabled\", \"private\", \"enabled\", \"public\"],\n      \"description\": \"The access level for the merge requests feature.\"\n    },\n    \"builds_access_level\": {\n      \"type\": \"string\",\n      \"enum\": [\"disabled\", \"private\", \"enabled\", \"public\"],\n      \"description\": \"The access level for CI/CD pipelines and builds.\"\n    },\n    \"wiki_access_level\": {\n      \"type\": \"string\",\n      \"enum\": [\"disabled\", \"private\", \"enabled\", \"public\"],\n      \"description\": \"The access level for the project wiki.\"\n    },\n    \"container_registry_access_level\": {\n      \"type\": \"string\",\n      \"enum\": [\"disabled\", \"private\", \"enabled\", \"public\"],\n      \"description\": \"The access level for the container registry.\"\n    },\n    \"pages_access_level\": {\n      \"type\": \"string\",\n      \"enum\": [\"disabled\", \"private\", \"enabled\", \"public\"],\n      \"description\": \"The access level for GitLab Pages.\"\n\
  \    },\n    \"permissions\": {\n      \"$ref\": \"#/$defs/Permissions\"\n    },\n    \"statistics\": {\n      \"$ref\": \"#/$defs/Statistics\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the project was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the project was last updated.\"\n    },\n    \"last_activity_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the last activity in the project.\"\n    }\n  },\n  \"$defs\": {\n    \"Namespace\": {\n      \"type\": \"object\",\n      \"description\": \"The namespace (user or group) that owns the project.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the namespace.\"\n        },\n        \"name\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The display name of the namespace.\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"The URL path of the namespace.\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"enum\": [\"user\", \"group\"],\n          \"description\": \"Whether the namespace belongs to a user or a group.\"\n        },\n        \"full_path\": {\n          \"type\": \"string\",\n          \"description\": \"The full path of the namespace.\"\n        },\n        \"parent_id\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The ID of the parent namespace for subgroups.\"\n        },\n        \"avatar_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL to the namespace avatar image.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uri\",\n          \"description\": \"URL to the namespace page on GitLab.\"\n        }\n      }\n    },\n    \"UserSummary\": {\n      \"type\": \"object\",\n      \"description\": \"A simplified representation of a GitLab user.\",\n      \"required\": [\"id\", \"username\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"blocked\", \"deactivated\"],\n          \"description\": \"The current state of the user account.\"\n        },\n        \"avatar_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n \
  \         \"description\": \"URL to the user's avatar image.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's profile on GitLab.\"\n        }\n      }\n    },\n    \"Permissions\": {\n      \"type\": \"object\",\n      \"description\": \"The access permissions the current user has on the project.\",\n      \"properties\": {\n        \"project_access\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"Direct project access level for the user.\",\n          \"properties\": {\n            \"access_level\": {\n              \"type\": \"integer\",\n              \"description\": \"Access level value (10=Guest, 20=Reporter, 30=Developer, 40=Maintainer, 50=Owner).\"\n            }\n          }\n        },\n        \"group_access\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"Group-inherited access level for the user.\",\n          \"\
  properties\": {\n            \"access_level\": {\n              \"type\": \"integer\",\n              \"description\": \"Access level value inherited from group membership.\"\n            }\n          }\n        }\n      }\n    },\n    \"Statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Storage and activity statistics for the project.\",\n      \"properties\": {\n        \"commit_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The total number of commits in the default branch.\"\n        },\n        \"storage_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total storage size in bytes.\"\n        },\n        \"repository_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Git repository size in bytes.\"\n        },\n        \"wiki_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"\
  description\": \"Wiki repository size in bytes.\"\n        },\n        \"lfs_objects_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"LFS objects size in bytes.\"\n        },\n        \"job_artifacts_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"CI/CD job artifacts size in bytes.\"\n        },\n        \"packages_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Packages registry size in bytes.\"\n        },\n        \"snippets_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Snippets size in bytes.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-project-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: GitLab Project
---
