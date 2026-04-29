---
description: A job represents a single execution of a job template, tracking the playbook run status, timing, and output.
layout: schema
name: Job
properties_list:
- description: The unique identifier of the job.
  name: id
  type: integer
- description: The name of the job.
  name: name
  type: string
- description: The current execution status of the job.
  name: status
  type: string
- description: Whether the job execution failed.
  name: failed
  type: boolean
- description: When the job execution started.
  name: started
  type: string
- description: When the job execution finished.
  name: finished
  type: string
- description: The elapsed time in seconds for job execution.
  name: elapsed
  type: number
- description: The ID of the job template that was executed.
  name: job_template
  type: integer
- description: The ID of the inventory used for this job.
  name: inventory
  type: integer
- description: The ID of the project used for this job.
  name: project
  type: integer
- description: The playbook that was executed.
  name: playbook
  type: string
- description: How the job was launched.
  name: launch_type
  type: string
- description: The date and time the job record was created.
  name: created
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-ansible-automation-platform-job-schema.json
slug: red-hat-ansible-automation-platform-job
source_filename: red-hat-ansible-automation-platform-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"description\": \"A job represents a single execution of a job template, tracking the playbook run status, timing, and output.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the job.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current execution status of the job.\"\n    },\n    \"failed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job execution failed.\"\n    },\n    \"started\": {\n      \"type\": \"string\",\n      \"description\": \"When the job execution started.\"\n    },\n    \"finished\": {\n      \"type\": \"string\",\n      \"description\": \"When the job execution finished.\"\n    },\n    \"elapsed\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"The elapsed time in seconds for job execution.\"\n    },\n    \"job_template\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the job template that was executed.\"\n    },\n    \"inventory\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the inventory used for this job.\"\n    },\n    \"project\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project used for this job.\"\n    },\n    \"playbook\": {\n      \"type\": \"string\",\n      \"description\": \"The playbook that was executed.\"\n    },\n    \"launch_type\": {\n      \"type\": \"string\",\n      \"description\": \"How the job was launched.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job record was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-automation-platform-job-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Job
---
