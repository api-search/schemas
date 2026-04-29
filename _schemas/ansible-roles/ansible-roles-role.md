---
description: An Ansible role published on Galaxy, containing tasks, handlers, defaults, templates, and metadata for reuse across playbooks.
layout: schema
name: Role
properties_list:
- description: Unique numeric identifier for the role.
  name: id
  type: integer
- description: Name of the role.
  name: name
  type: string
- description: Galaxy namespace (usually GitHub username) of the role author.
  name: namespace
  type: string
- description: Short description of what the role does.
  name: description
  type: string
- description: GitHub username of the role author.
  name: github_user
  type: string
- description: GitHub repository name for this role.
  name: github_repo
  type: string
- description: Default branch for this role's repository.
  name: github_branch
  type: string
- description: Total number of times this role has been downloaded.
  name: download_count
  type: integer
- description: Number of GitHub stars for this role.
  name: stargazers_count
  type: integer
- description: Number of GitHub forks for this role.
  name: forks_count
  type: integer
- description: Number of open GitHub issues for this role.
  name: open_issues_count
  type: integer
- description: Minimum Ansible version required by this role.
  name: min_ansible_version
  type: string
- description: Software license for this role.
  name: license
  type: string
- description: When this role was first published to Galaxy.
  name: created
  type: string
- description: When this role was last updated.
  name: modified
  type: string
provider_name: Ansible Roles
provider_slug: ansible-roles
schema_file: json-schema/ansible-roles-role-schema.json
slug: ansible-roles-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/json-schema/ansible-roles-role-schema.json\",\n  \"title\": \"Role\",\n  \"description\": \"An Ansible role published on Galaxy, containing tasks, handlers, defaults, templates, and metadata for reuse across playbooks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"integer\", \"description\": \"Unique numeric identifier for the role.\", \"example\": 500123},\n    \"name\": {\"type\": \"string\", \"description\": \"Name of the role.\", \"example\": \"nginx\"},\n    \"namespace\": {\"type\": \"string\", \"description\": \"Galaxy namespace (usually GitHub username) of the role author.\", \"example\": \"geerlingguy\"},\n    \"description\": {\"type\": \"string\", \"description\": \"Short description of what the role does.\", \"example\": \"Installs and configures Nginx web server.\"},\n    \"\
  github_user\": {\"type\": \"string\", \"description\": \"GitHub username of the role author.\", \"example\": \"geerlingguy\"},\n    \"github_repo\": {\"type\": \"string\", \"description\": \"GitHub repository name for this role.\", \"example\": \"ansible-role-nginx\"},\n    \"github_branch\": {\"type\": \"string\", \"description\": \"Default branch for this role's repository.\", \"example\": \"master\"},\n    \"download_count\": {\"type\": \"integer\", \"description\": \"Total number of times this role has been downloaded.\", \"example\": 1250000},\n    \"stargazers_count\": {\"type\": \"integer\", \"description\": \"Number of GitHub stars for this role.\", \"example\": 1800},\n    \"forks_count\": {\"type\": \"integer\", \"description\": \"Number of GitHub forks for this role.\", \"example\": 750},\n    \"open_issues_count\": {\"type\": \"integer\", \"description\": \"Number of open GitHub issues for this role.\", \"example\": 12},\n    \"min_ansible_version\": {\"type\": \"string\",\
  \ \"description\": \"Minimum Ansible version required by this role.\", \"example\": \"2.8\"},\n    \"license\": {\"type\": \"string\", \"description\": \"Software license for this role.\", \"example\": \"MIT\"},\n    \"created\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"When this role was first published to Galaxy.\", \"example\": \"2015-01-01T00:00:00Z\"},\n    \"modified\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"When this role was last updated.\", \"example\": \"2026-04-01T00:00:00Z\"}\n  },\n  \"required\": [\"id\", \"name\", \"namespace\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/json-schema/ansible-roles-role-schema.json
tags:
- Ansible
- Automation
- Collections
- Configuration Management
- DevOps
- Infrastructure As Code
- Roles
title: Role
---
