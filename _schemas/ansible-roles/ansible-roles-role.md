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
