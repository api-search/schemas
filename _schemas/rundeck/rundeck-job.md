---
description: Represents an automation job in Rundeck. Jobs define the steps to execute, target nodes, schedule, and access control. Jobs are organized within projects and can be triggered manually, via API, schedule, or webhook.
layout: schema
name: Rundeck Job
properties_list:
- description: Unique job identifier (UUID).
  name: id
  type: string
- description: The job name. Must be unique within its group and project.
  name: name
  type: string
- description: The job group path using forward slashes (e.g., 'ops/deploy'). Used for organizing jobs hierarchically.
  name: group
  type: string
- description: The name of the Rundeck project that owns this job.
  name: project
  type: string
- description: Human-readable description of what this job does.
  name: description
  type: string
- description: API self-link URL for this job resource.
  name: href
  type: string
- description: Web UI permalink to view this job.
  name: permalink
  type: string
- description: Whether this job has a schedule configured.
  name: scheduled
  type: boolean
- description: Whether the job's schedule is currently active.
  name: scheduleEnabled
  type: boolean
- description: Whether the job is enabled and can be executed.
  name: enabled
  type: boolean
- description: Average execution duration in milliseconds based on recent executions.
  name: averageDuration
  type: integer
- description: Job input options (parameters) that can be supplied at runtime.
  name: options
  type: array
- description: Whether the node filter can be overridden at execution time.
  name: nodeFilterEditable
  type: boolean
- description: Default log level for job executions.
  name: loglevel
  type: string
provider_name: Rundeck
provider_slug: rundeck
schema_file: json-schema/rundeck-job-schema.json
slug: rundeck-job
source_filename: rundeck-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rundeck.com/schemas/rundeck/job.json\",\n  \"title\": \"Rundeck Job\",\n  \"description\": \"Represents an automation job in Rundeck. Jobs define the steps to execute, target nodes, schedule, and access control. Jobs are organized within projects and can be triggered manually, via API, schedule, or webhook.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"project\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique job identifier (UUID).\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The job name. Must be unique within its group and project.\",\n      \"minLength\": 1\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"The job group path using forward slashes (e.g., 'ops/deploy'). Used for organizing jobs hierarchically.\"\n    },\n\
  \    \"project\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Rundeck project that owns this job.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what this job does.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API self-link URL for this job resource.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web UI permalink to view this job.\"\n    },\n    \"scheduled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this job has a schedule configured.\"\n    },\n    \"scheduleEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job's schedule is currently active.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job is enabled and can be executed.\"\
  ,\n      \"default\": true\n    },\n    \"averageDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Average execution duration in milliseconds based on recent executions.\",\n      \"minimum\": 0\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"description\": \"Job input options (parameters) that can be supplied at runtime.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/JobOption\"\n      }\n    },\n    \"nodeFilterEditable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the node filter can be overridden at execution time.\"\n    },\n    \"loglevel\": {\n      \"type\": \"string\",\n      \"description\": \"Default log level for job executions.\",\n      \"enum\": [\"DEBUG\", \"VERBOSE\", \"INFO\", \"WARN\", \"ERROR\"]\n    }\n  },\n  \"$defs\": {\n    \"JobOption\": {\n      \"type\": \"object\",\n      \"description\": \"An input option for a Rundeck job, allowing parameterization of job executions.\",\n      \"required\":\
  \ [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The option name used in the argument string.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of this option.\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this option must be provided.\",\n          \"default\": false\n        },\n        \"defaultValue\": {\n          \"type\": \"string\",\n          \"description\": \"Default value if none is provided.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Option data type.\",\n          \"enum\": [\"text\", \"file\"]\n        },\n        \"secure\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a secure/password option (value is masked in logs).\",\n          \"default\": false\n        },\n\
  \        \"values\": {\n          \"type\": \"array\",\n          \"description\": \"List of allowed values for this option.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"regex\": {\n          \"type\": \"string\",\n          \"description\": \"Regular expression pattern that input values must match.\"\n        }\n      }\n    },\n    \"Execution\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a single execution instance of a Rundeck job or ad hoc command.\",\n      \"required\": [\"id\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique execution identifier.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current execution status.\",\n          \"enum\": [\"running\", \"succeeded\", \"failed\", \"aborted\", \"timedout\", \"failed-with-retry\", \"scheduled\"]\n        },\n        \"project\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Project name for this execution.\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"Username that triggered this execution.\"\n        },\n        \"dateStarted\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"unixtime\": {\n              \"type\": \"integer\",\n              \"description\": \"Unix timestamp in milliseconds.\"\n            },\n            \"date\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"ISO 8601 datetime.\"\n            }\n          }\n        },\n        \"dateEnded\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"unixtime\": {\n              \"type\": \"integer\"\n            },\n            \"date\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            }\n          }\n     \
  \   },\n        \"argstring\": {\n          \"type\": \"string\",\n          \"description\": \"Job argument string used for this execution.\"\n        },\n        \"serverUUID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"UUID of the Rundeck server cluster member that ran this execution.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"permalink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rundeck/refs/heads/main/json-schema/rundeck-job-schema.json
tags:
- Automation
- DevOps
- Job Scheduling
- Orchestration
- Workflow
- Runbook
- Open Source
- IT Operations
title: Rundeck Job
---
