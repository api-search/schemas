---
description: An Ansible playbook job representing a single execution of a job template, including status, output, and configuration details.
layout: schema
name: PlaybookJob
properties_list:
- description: Unique numeric identifier for the job.
  name: id
  type: integer
- description: Name of the job template that spawned this job.
  name: name
  type: string
- description: Current job status.
  name: status
  type: string
- description: Playbook file executed by this job.
  name: playbook
  type: string
- description: Timestamp when the job started executing.
  name: started
  type: string
- description: Timestamp when the job finished.
  name: finished
  type: string
- description: Job duration in seconds.
  name: elapsed
  type: number
- description: Type of Ansible job.
  name: job_type
  type: string
- description: How the job was launched.
  name: launch_type
  type: string
- description: Ansible verbosity level (0-5).
  name: verbosity
  type: integer
- description: Host pattern limit applied to this job run.
  name: limit
  type: string
- description: Extra variables passed to the playbook as a JSON string.
  name: extra_vars
  type: string
- description: ID of the inventory used by this job.
  name: inventory
  type: integer
- description: ID of the project containing the playbook.
  name: project
  type: integer
- description: Error traceback if the job failed.
  name: result_traceback
  type: string
- description: Timestamp when the job record was created.
  name: created
  type: string
- description: Timestamp when the job record was last modified.
  name: modified
  type: string
provider_name: Ansible Playbooks
provider_slug: ansible-playbooks
schema_file: json-schema/ansible-playbooks-playbook-job-schema.json
slug: ansible-playbooks-playbook-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/json-schema/ansible-playbooks-playbook-job-schema.json\",\n  \"title\": \"PlaybookJob\",\n  \"description\": \"An Ansible playbook job representing a single execution of a job template, including status, output, and configuration details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"integer\", \"description\": \"Unique numeric identifier for the job.\", \"example\": 500123},\n    \"name\": {\"type\": \"string\", \"description\": \"Name of the job template that spawned this job.\", \"example\": \"Deploy Web Application\"},\n    \"status\": {\"type\": \"string\", \"enum\": [\"new\", \"pending\", \"waiting\", \"running\", \"successful\", \"failed\", \"error\", \"canceled\"], \"description\": \"Current job status.\", \"example\": \"successful\"},\n    \"playbook\": {\"type\": \"string\"\
  , \"description\": \"Playbook file executed by this job.\", \"example\": \"site.yml\"},\n    \"started\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp when the job started executing.\", \"example\": \"2026-04-19T14:00:00Z\"},\n    \"finished\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp when the job finished.\", \"example\": \"2026-04-19T14:05:00Z\"},\n    \"elapsed\": {\"type\": \"number\", \"description\": \"Job duration in seconds.\", \"example\": 300.5},\n    \"job_type\": {\"type\": \"string\", \"enum\": [\"run\", \"check\", \"scan\"], \"description\": \"Type of Ansible job.\", \"example\": \"run\"},\n    \"launch_type\": {\"type\": \"string\", \"enum\": [\"manual\", \"relaunch\", \"callback\", \"scheduled\", \"dependency\", \"workflow\", \"sync\", \"scm\"], \"description\": \"How the job was launched.\", \"example\": \"manual\"},\n    \"verbosity\": {\"type\": \"integer\", \"minimum\": 0, \"maximum\": 5, \"description\"\
  : \"Ansible verbosity level (0-5).\", \"example\": 0},\n    \"limit\": {\"type\": \"string\", \"description\": \"Host pattern limit applied to this job run.\", \"example\": \"web-servers\"},\n    \"extra_vars\": {\"type\": \"string\", \"description\": \"Extra variables passed to the playbook as a JSON string.\", \"example\": \"{\\\"env\\\": \\\"production\\\"}\"},\n    \"inventory\": {\"type\": \"integer\", \"description\": \"ID of the inventory used by this job.\", \"example\": 42},\n    \"project\": {\"type\": \"integer\", \"description\": \"ID of the project containing the playbook.\", \"example\": 7},\n    \"result_traceback\": {\"type\": \"string\", \"description\": \"Error traceback if the job failed.\", \"example\": \"\"},\n    \"created\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp when the job record was created.\", \"example\": \"2026-04-19T13:59:00Z\"},\n    \"modified\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"\
  Timestamp when the job record was last modified.\", \"example\": \"2026-04-19T14:05:00Z\"}\n  },\n  \"required\": [\"id\", \"name\", \"status\", \"playbook\", \"job_type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/json-schema/ansible-playbooks-playbook-job-schema.json
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure As Code
- Orchestration
- Playbooks
title: PlaybookJob
---
