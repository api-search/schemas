---
description: A CircleCI pipeline represents a full CI/CD execution triggered by a code change, API call, or schedule. It contains one or more workflows that organize and run jobs.
layout: schema
name: CircleCI Pipeline
properties_list:
- description: The unique identifier of the pipeline
  name: id
  type: string
- description: Errors that occurred during pipeline setup
  name: errors
  type: array
- description: The project slug in vcs-slug/org-name/repo-name format
  name: project_slug
  type: string
- description: When the pipeline was last updated
  name: updated_at
  type: string
- description: The monotonically increasing pipeline number
  name: number
  type: integer
- description: The current state of the pipeline
  name: state
  type: string
- description: When the pipeline was created
  name: created_at
  type: string
- description: ''
  name: trigger
  type: object
- description: Parameters passed when triggering the pipeline
  name: trigger_parameters
  type: object
- description: ''
  name: vcs
  type: object
provider_name: CircleCI
provider_slug: circleci
schema_file: json-schema/circleci-pipeline-schema.json
slug: circleci-pipeline
source_filename: circleci-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://circleci.com/schemas/circleci/pipeline.json\",\n  \"title\": \"CircleCI Pipeline\",\n  \"description\": \"A CircleCI pipeline represents a full CI/CD execution triggered by a code change, API call, or schedule. It contains one or more workflows that organize and run jobs.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"state\", \"number\", \"created_at\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the pipeline\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PipelineError\"\n      },\n      \"description\": \"Errors that occurred during pipeline setup\"\n    },\n    \"project_slug\": {\n      \"type\": \"string\",\n      \"description\": \"The project slug in vcs-slug/org-name/repo-name format\",\n      \"pattern\": \"^(gh|github|bb|bitbucket)/[^/]+/[^/]+$\"\
  \n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the pipeline was last updated\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The monotonically increasing pipeline number\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"created\", \"errored\", \"setup-pending\", \"setup\", \"pending\"],\n      \"description\": \"The current state of the pipeline\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the pipeline was created\"\n    },\n    \"trigger\": {\n      \"$ref\": \"#/$defs/Trigger\"\n    },\n    \"trigger_parameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Parameters passed when triggering the pipeline\"\n    },\n    \"vcs\": {\n      \"$ref\": \"#/$defs/VCSInfo\"\n    }\n  },\n  \"$defs\"\
  : {\n    \"PipelineError\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"config\", \"config-fetch\", \"timeout\", \"permission\", \"other\"],\n          \"description\": \"The type of error that occurred\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable error message\"\n        }\n      },\n      \"required\": [\"type\", \"message\"]\n    },\n    \"Trigger\": {\n      \"type\": \"object\",\n      \"description\": \"Information about what triggered the pipeline\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"webhook\", \"explicit\", \"api\", \"schedule\"],\n          \"description\": \"The type of trigger that started this pipeline\"\n        },\n        \"received_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When\
  \ the trigger was received\"\n        },\n        \"actor\": {\n          \"$ref\": \"#/$defs/Actor\"\n        }\n      }\n    },\n    \"Actor\": {\n      \"type\": \"object\",\n      \"description\": \"The user or system that triggered the pipeline\",\n      \"properties\": {\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"The login name of the actor\"\n        },\n        \"avatar_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the actor's avatar\"\n        }\n      }\n    },\n    \"VCSInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Version control system information associated with the pipeline\",\n      \"properties\": {\n        \"provider_name\": {\n          \"type\": \"string\",\n          \"enum\": [\"github\", \"bitbucket\"],\n          \"description\": \"The VCS provider name\"\n        },\n        \"origin_repository_url\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"uri\",\n          \"description\": \"The URL of the origin repository\"\n        },\n        \"target_repository_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the target repository\"\n        },\n        \"revision\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9a-f]{40}$\",\n          \"description\": \"The full SHA-1 commit hash\"\n        },\n        \"branch\": {\n          \"type\": \"string\",\n          \"description\": \"The branch name\"\n        },\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"The tag name, if applicable\"\n        },\n        \"commit\": {\n          \"$ref\": \"#/$defs/Commit\"\n        }\n      }\n    },\n    \"Commit\": {\n      \"type\": \"object\",\n      \"description\": \"Commit information associated with the pipeline\",\n      \"properties\": {\n        \"subject\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The commit message subject line\"\n        },\n        \"body\": {\n          \"type\": \"string\",\n          \"description\": \"The commit message body\"\n        },\n        \"author\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The commit author name\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n              \"description\": \"The commit author email\"\n            }\n          },\n          \"description\": \"The commit author\"\n        },\n        \"committer\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The committer name\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n  \
  \            \"description\": \"The committer email\"\n            }\n          },\n          \"description\": \"The committer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/json-schema/circleci-pipeline-schema.json
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
title: CircleCI Pipeline
---
