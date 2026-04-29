---
description: A GitLab CI/CD pipeline that runs automated jobs defined in a .gitlab-ci.yml configuration file.
layout: schema
name: GitLab Pipeline
properties_list:
- description: The unique identifier of the pipeline.
  name: id
  type: integer
- description: The project-scoped sequential ID of the pipeline.
  name: iid
  type: integer
- description: The ID of the project the pipeline belongs to.
  name: project_id
  type: integer
- description: The user-defined name of the pipeline.
  name: name
  type:
  - string
  - 'null'
- description: The current execution status of the pipeline.
  name: status
  type: string
- description: The source that triggered the pipeline.
  name: source
  type: string
- description: The branch name, tag name, or commit SHA the pipeline runs on.
  name: ref
  type: string
- description: The full SHA of the commit the pipeline runs on.
  name: sha
  type: string
- description: Whether the pipeline was triggered by a tag push.
  name: tag
  type: boolean
- description: YAML configuration validation errors, if any.
  name: yaml_errors
  type:
  - string
  - 'null'
- description: ''
  name: user
  type: object
- description: The URL to view the pipeline in a browser.
  name: web_url
  type: string
- description: The SHA of the commit before the pipeline was triggered.
  name: before_sha
  type: string
- description: The total duration of the pipeline in seconds.
  name: duration
  type:
  - integer
  - 'null'
- description: The time in seconds the pipeline spent in the queue before starting.
  name: queued_duration
  type:
  - number
  - 'null'
- description: The code coverage percentage reported by the pipeline.
  name: coverage
  type:
  - string
  - 'null'
- description: Whether the pipeline has been archived.
  name: archived
  type: boolean
- description: The date and time the pipeline was created.
  name: created_at
  type: string
- description: The date and time the pipeline was last updated.
  name: updated_at
  type: string
- description: The date and time the pipeline started execution.
  name: started_at
  type:
  - string
  - 'null'
- description: The date and time the pipeline finished execution.
  name: finished_at
  type:
  - string
  - 'null'
- description: The date and time of the commit that triggered the pipeline.
  name: committed_at
  type:
  - string
  - 'null'
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-pipeline-schema.json
slug: gitlab-pipeline
source_filename: gitlab-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gitlab.com/schemas/gitlab/pipeline.json\",\n  \"title\": \"GitLab Pipeline\",\n  \"description\": \"A GitLab CI/CD pipeline that runs automated jobs defined in a .gitlab-ci.yml configuration file.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"project_id\", \"status\", \"ref\", \"sha\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the pipeline.\"\n    },\n    \"iid\": {\n      \"type\": \"integer\",\n      \"description\": \"The project-scoped sequential ID of the pipeline.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project the pipeline belongs to.\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user-defined name of the pipeline.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"\
  enum\": [\"created\", \"waiting_for_resource\", \"preparing\", \"pending\", \"running\", \"success\", \"failed\", \"canceled\", \"skipped\", \"manual\", \"scheduled\"],\n      \"description\": \"The current execution status of the pipeline.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\"push\", \"web\", \"trigger\", \"schedule\", \"api\", \"external\", \"pipeline\", \"chat\", \"webide\", \"merge_request_event\", \"external_pull_request_event\", \"parent_pipeline\", \"ondemand_dast_scan\", \"ondemand_dast_validation\"],\n      \"description\": \"The source that triggered the pipeline.\"\n    },\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"The branch name, tag name, or commit SHA the pipeline runs on.\"\n    },\n    \"sha\": {\n      \"type\": \"string\",\n      \"description\": \"The full SHA of the commit the pipeline runs on.\",\n      \"pattern\": \"^[0-9a-f]{40}$\"\n    },\n    \"tag\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether the pipeline was triggered by a tag push.\"\n    },\n    \"yaml_errors\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"YAML configuration validation errors, if any.\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/UserSummary\"\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to view the pipeline in a browser.\"\n    },\n    \"before_sha\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA of the commit before the pipeline was triggered.\"\n    },\n    \"duration\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The total duration of the pipeline in seconds.\"\n    },\n    \"queued_duration\": {\n      \"type\": [\"number\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The time in seconds the pipeline spent in the queue before starting.\"\n    },\n    \"coverage\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"The code coverage percentage reported by the pipeline.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the pipeline has been archived.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pipeline was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pipeline was last updated.\"\n    },\n    \"started_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pipeline started execution.\"\n    },\n    \"finished_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the pipeline finished execution.\"\n    },\n    \"committed_at\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the commit that triggered the pipeline.\"\n    }\n  },\n  \"$defs\": {\n    \"UserSummary\": {\n      \"type\": \"object\",\n      \"description\": \"A simplified representation of the GitLab user who triggered the pipeline.\",\n      \"required\": [\"id\", \"username\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"blocked\", \"deactivated\"],\n          \"description\": \"The current state of the user account.\"\n        },\n        \"avatar_url\": {\n\
  \          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"web_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's GitLab profile page.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-pipeline-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: GitLab Pipeline
---
