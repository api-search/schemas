---
description: A GitHub repository containing source code, issues, pull requests, and other project resources.
layout: schema
name: GitHub Repository
properties_list:
- description: The unique identifier of the repository.
  name: id
  type: integer
- description: The GraphQL node ID for the repository.
  name: node_id
  type: string
- description: The name of the repository without the owner prefix.
  name: name
  type: string
- description: The full name of the repository in owner/name format.
  name: full_name
  type: string
- description: ''
  name: owner
  type: object
- description: Whether the repository is private.
  name: private
  type: boolean
- description: The URL of the repository on GitHub.
  name: html_url
  type: string
- description: A short description of the repository.
  name: description
  type:
  - string
  - 'null'
- description: Whether the repository is a fork of another repository.
  name: fork
  type: boolean
- description: The API URL for the repository.
  name: url
  type: string
- description: The date and time the repository was created.
  name: created_at
  type: string
- description: The date and time the repository was last updated.
  name: updated_at
  type: string
- description: The date and time of the last push to the repository.
  name: pushed_at
  type: string
- description: The URL of the repository's homepage.
  name: homepage
  type:
  - string
  - 'null'
- description: The size of the repository in kilobytes.
  name: size
  type: integer
- description: The number of stars the repository has received.
  name: stargazers_count
  type: integer
- description: The number of watchers on the repository.
  name: watchers_count
  type: integer
- description: The primary programming language of the repository.
  name: language
  type:
  - string
  - 'null'
- description: The number of forks of the repository.
  name: forks_count
  type: integer
- description: The number of open issues in the repository.
  name: open_issues_count
  type: integer
- description: The default branch of the repository.
  name: default_branch
  type: string
- description: The visibility level of the repository.
  name: visibility
  type: string
- description: The topics (tags) associated with the repository.
  name: topics
  type: array
- description: Whether the repository has issues enabled.
  name: has_issues
  type: boolean
- description: Whether the repository has projects enabled.
  name: has_projects
  type: boolean
- description: Whether the repository has the wiki enabled.
  name: has_wiki
  type: boolean
- description: Whether the repository has GitHub Pages enabled.
  name: has_pages
  type: boolean
- description: Whether the repository has downloads enabled.
  name: has_downloads
  type: boolean
- description: Whether the repository has discussions enabled.
  name: has_discussions
  type: boolean
- description: Whether the repository is archived and read-only.
  name: archived
  type: boolean
- description: Whether the repository is disabled.
  name: disabled
  type: boolean
- description: Whether the repository is a template repository.
  name: is_template
  type: boolean
- description: Whether forking is allowed on the repository.
  name: allow_forking
  type: boolean
- description: ''
  name: license
  type: object
- description: ''
  name: permissions
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repository-schema.json
slug: github-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/schemas/github/repository.json\",\n  \"title\": \"GitHub Repository\",\n  \"description\": \"A GitHub repository containing source code, issues, pull requests, and other project resources.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"full_name\", \"owner\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the repository.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID for the repository.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the repository without the owner prefix.\",\n      \"pattern\": \"^[a-zA-Z0-9._-]+$\"\n    },\n    \"full_name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the repository in owner/name format.\",\n      \"pattern\": \"^[a-zA-Z0-9._-]+/[a-zA-Z0-9._-]+$\"\
  \n    },\n    \"owner\": {\n      \"$ref\": \"#/$defs/SimpleUser\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is private.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the repository on GitHub.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A short description of the repository.\",\n      \"maxLength\": 350\n    },\n    \"fork\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is a fork of another repository.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the repository.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the repository was created.\"\n    },\n    \"updated_at\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the repository was last updated.\"\n    },\n    \"pushed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the last push to the repository.\"\n    },\n    \"homepage\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URL of the repository's homepage.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The size of the repository in kilobytes.\"\n    },\n    \"stargazers_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of stars the repository has received.\"\n    },\n    \"watchers_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of watchers on the repository.\"\n    },\n    \"language\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"description\": \"The primary programming language of the repository.\"\n    },\n    \"forks_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of forks of the repository.\"\n    },\n    \"open_issues_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of open issues in the repository.\"\n    },\n    \"default_branch\": {\n      \"type\": \"string\",\n      \"description\": \"The default branch of the repository.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\", \"internal\"],\n      \"description\": \"The visibility level of the repository.\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"The topics (tags) associated with the repository.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"has_issues\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether the repository has issues enabled.\"\n    },\n    \"has_projects\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository has projects enabled.\"\n    },\n    \"has_wiki\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository has the wiki enabled.\"\n    },\n    \"has_pages\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository has GitHub Pages enabled.\"\n    },\n    \"has_downloads\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository has downloads enabled.\"\n    },\n    \"has_discussions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository has discussions enabled.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is archived and read-only.\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is disabled.\"\n    },\n\
  \    \"is_template\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is a template repository.\"\n    },\n    \"allow_forking\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether forking is allowed on the repository.\"\n    },\n    \"license\": {\n      \"$ref\": \"#/$defs/License\"\n    },\n    \"permissions\": {\n      \"$ref\": \"#/$defs/Permissions\"\n    }\n  },\n  \"$defs\": {\n    \"SimpleUser\": {\n      \"type\": \"object\",\n      \"description\": \"A simplified representation of a GitHub user.\",\n      \"required\": [\"login\", \"id\"],\n      \"properties\": {\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for the user.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n\
  \        },\n        \"avatar_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"html_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's GitHub profile.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Organization\", \"Bot\"],\n          \"description\": \"The type of account.\"\n        },\n        \"site_admin\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user is a GitHub site administrator.\"\n        }\n      }\n    },\n    \"License\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The license associated with the repository.\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The SPDX license key.\"\n        },\n        \"name\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"The full name of the license.\"\n        },\n        \"spdx_id\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The SPDX identifier for the license.\"\n        },\n        \"url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL to the license on api.github.com.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        }\n      }\n    },\n    \"Permissions\": {\n      \"type\": \"object\",\n      \"description\": \"The permissions the authenticated user has on the repository.\",\n      \"properties\": {\n        \"admin\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has admin access.\"\n        },\n        \"maintain\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has maintain access.\"\
  \n        },\n        \"push\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has push (write) access.\"\n        },\n        \"triage\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has triage access.\"\n        },\n        \"pull\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user has pull (read) access.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repository-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: GitHub Repository
---
