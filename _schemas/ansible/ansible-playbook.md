---
description: An Ansible playbook — a YAML file containing one or more plays that map a group of hosts to a set of roles and tasks.
layout: schema
name: Playbook
properties_list:
- description: Human-readable name for the playbook play.
  name: name
  type: string
- description: Host or group pattern targeted by this play.
  name: hosts
  type: string
- description: Whether to run tasks with privilege escalation (sudo).
  name: become
  type: boolean
- description: User to become when privilege escalation is enabled.
  name: become_user
  type: string
- description: Whether to gather system facts before running tasks.
  name: gather_facts
  type: boolean
- description: Variables defined at the play level.
  name: vars
  type: object
- description: List of roles applied to hosts in this play.
  name: roles
  type: array
- description: List of tasks executed in this play.
  name: tasks
  type: array
- description: Handlers triggered by task notifications.
  name: handlers
  type: array
- description: Tags for selective task execution.
  name: tags
  type: array
provider_name: Ansible
provider_slug: ansible
schema_file: json-schema/ansible-playbook-schema.json
slug: ansible-playbook
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure As Code
- Open Source
- Orchestration
- Red Hat
title: Playbook
---
