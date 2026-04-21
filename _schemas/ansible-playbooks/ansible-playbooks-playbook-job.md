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
