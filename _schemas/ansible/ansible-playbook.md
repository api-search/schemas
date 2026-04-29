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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/json-schema/ansible-playbook-schema.json\",\n  \"title\": \"Playbook\",\n  \"description\": \"An Ansible playbook — a YAML file containing one or more plays that map a group of hosts to a set of roles and tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\"type\": \"string\", \"description\": \"Human-readable name for the playbook play.\", \"example\": \"Deploy Web Application\"},\n    \"hosts\": {\"type\": \"string\", \"description\": \"Host or group pattern targeted by this play.\", \"example\": \"web-servers\"},\n    \"become\": {\"type\": \"boolean\", \"description\": \"Whether to run tasks with privilege escalation (sudo).\", \"example\": true},\n    \"become_user\": {\"type\": \"string\", \"description\": \"User to become when privilege escalation is enabled.\", \"example\": \"root\"},\n    \"\
  gather_facts\": {\"type\": \"boolean\", \"description\": \"Whether to gather system facts before running tasks.\", \"example\": true},\n    \"vars\": {\"type\": \"object\", \"description\": \"Variables defined at the play level.\", \"additionalProperties\": true},\n    \"roles\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}, \"description\": \"List of roles applied to hosts in this play.\", \"example\": [\"nginx\", \"app-deploy\"]},\n    \"tasks\": {\"type\": \"array\", \"description\": \"List of tasks executed in this play.\", \"items\": {\"$ref\": \"#/$defs/Task\"}},\n    \"handlers\": {\"type\": \"array\", \"description\": \"Handlers triggered by task notifications.\", \"items\": {\"$ref\": \"#/$defs/Task\"}},\n    \"tags\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}, \"description\": \"Tags for selective task execution.\", \"example\": [\"deploy\", \"web\"]}\n  },\n  \"required\": [\"hosts\"],\n  \"$defs\": {\n    \"Task\": {\n      \"type\": \"object\",\n \
  \     \"properties\": {\n        \"name\": {\"type\": \"string\", \"description\": \"Human-readable task description.\", \"example\": \"Install Nginx\"},\n        \"module\": {\"type\": \"string\", \"description\": \"Ansible module name used by this task.\", \"example\": \"ansible.builtin.package\"},\n        \"when\": {\"type\": \"string\", \"description\": \"Conditional expression for task execution.\", \"example\": \"ansible_os_family == 'RedHat'\"},\n        \"tags\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}, \"description\": \"Tags associated with this task.\"},\n        \"notify\": {\"type\": \"string\", \"description\": \"Handler name to notify upon task change.\", \"example\": \"restart nginx\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/json-schema/ansible-playbook-schema.json
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
