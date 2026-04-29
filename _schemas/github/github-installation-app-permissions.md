---
description: The permissions granted to the user access token.
layout: schema
name: app-permissions
properties_list:
- description: The level of permission to grant the access token for GitHub Actions workflows, workflow runs, and artifacts.
  name: actions
  type: string
- description: The level of permission to grant the access token for repository creation, deletion, settings, teams, and collaborators creation.
  name: administration
  type: string
- description: The level of permission to grant the access token for checks on code.
  name: checks
  type: string
- description: The level of permission to grant the access token to create, edit, delete, and list Codespaces.
  name: codespaces
  type: string
- description: The level of permission to grant the access token for repository contents, commits, branches, downloads, releases, and merges.
  name: contents
  type: string
- description: The leve of permission to grant the access token to manage Dependabot secrets.
  name: dependabot_secrets
  type: string
- description: The level of permission to grant the access token for deployments and deployment statuses.
  name: deployments
  type: string
- description: The level of permission to grant the access token for managing repository environments.
  name: environments
  type: string
- description: The level of permission to grant the access token for issues and related comments, assignees, labels, and milestones.
  name: issues
  type: string
- description: The level of permission to grant the access token to search repositories, list collaborators, and access repository metadata.
  name: metadata
  type: string
- description: The level of permission to grant the access token for packages published to GitHub Packages.
  name: packages
  type: string
- description: The level of permission to grant the access token to retrieve Pages statuses, configuration, and builds, as well as create new builds.
  name: pages
  type: string
- description: The level of permission to grant the access token for pull requests and related comments, assignees, labels, milestones, and merges.
  name: pull_requests
  type: string
- description: The level of permission to grant the access token to manage the post-receive hooks for a repository.
  name: repository_hooks
  type: string
- description: The level of permission to grant the access token to manage repository projects, columns, and cards.
  name: repository_projects
  type: string
- description: The level of permission to grant the access token to view and manage secret scanning alerts.
  name: secret_scanning_alerts
  type: string
- description: The level of permission to grant the access token to manage repository secrets.
  name: secrets
  type: string
- description: The level of permission to grant the access token to view and manage security events like code scanning alerts.
  name: security_events
  type: string
- description: The level of permission to grant the access token to manage just a single file.
  name: single_file
  type: string
- description: The level of permission to grant the access token for commit statuses.
  name: statuses
  type: string
- description: The level of permission to grant the access token to manage Dependabot alerts.
  name: vulnerability_alerts
  type: string
- description: The level of permission to grant the access token to update GitHub Actions workflow files.
  name: workflows
  type: string
- description: The level of permission to grant the access token for organization teams and members.
  name: members
  type: string
- description: The level of permission to grant the access token to manage access to an organization.
  name: organization_administration
  type: string
- description: The level of permission to grant the access token for custom repository roles management.
  name: organization_custom_roles
  type: string
- description: 'The level of permission to grant the access token for managing access to GitHub Copilot for members of an organization with a Copilot Business subscription. This property is in beta and is subject to '
  name: organization_copilot_seat_management
  type: string
- description: The level of permission to grant the access token to view and manage announcement banners for an organization.
  name: organization_announcement_banners
  type: string
- description: The level of permission to grant the access token to view events triggered by an activity in an organization.
  name: organization_events
  type: string
- description: The level of permission to grant the access token to manage the post-receive hooks for an organization.
  name: organization_hooks
  type: string
- description: The level of permission to grant the access token for viewing and managing fine-grained personal access token requests to an organization.
  name: organization_personal_access_tokens
  type: string
- description: The level of permission to grant the access token for viewing and managing fine-grained personal access tokens that have been approved by an organization.
  name: organization_personal_access_token_requests
  type: string
- description: The level of permission to grant the access token for viewing an organization's plan.
  name: organization_plan
  type: string
- description: The level of permission to grant the access token to manage organization projects and projects beta (where available).
  name: organization_projects
  type: string
- description: The level of permission to grant the access token for organization packages published to GitHub Packages.
  name: organization_packages
  type: string
- description: The level of permission to grant the access token to manage organization secrets.
  name: organization_secrets
  type: string
- description: The level of permission to grant the access token to view and manage GitHub Actions self-hosted runners available to an organization.
  name: organization_self_hosted_runners
  type: string
- description: The level of permission to grant the access token to view and manage users blocked by the organization.
  name: organization_user_blocking
  type: string
- description: The level of permission to grant the access token to manage team discussions and related comments.
  name: team_discussions
  type: string
- description: The level of permission to grant the access token to manage the email addresses belonging to a user.
  name: email_addresses
  type: string
- description: The level of permission to grant the access token to manage the followers belonging to a user.
  name: followers
  type: string
- description: The level of permission to grant the access token to manage git SSH keys.
  name: git_ssh_keys
  type: string
- description: The level of permission to grant the access token to view and manage GPG keys belonging to a user.
  name: gpg_keys
  type: string
- description: The level of permission to grant the access token to view and manage interaction limits on a repository.
  name: interaction_limits
  type: string
- description: The level of permission to grant the access token to manage the profile settings belonging to a user.
  name: profile
  type: string
- description: The level of permission to grant the access token to list and manage repositories a user is starring.
  name: starring
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-installation-app-permissions-schema.json
slug: github-installation-app-permissions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-app-permissions-schema.json\",\n  \"title\": \"app-permissions\",\n  \"description\": \"The permissions granted to the user access token.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for GitHub Actions workflows, workflow runs, and artifacts.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"administration\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for repository creation, deletion, settings, teams, and collaborators creation.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n  \
  \  \"checks\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for checks on code.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"codespaces\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to create, edit, delete, and list Codespaces.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"contents\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for repository contents, commits, branches, downloads, releases, and merges.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"dependabot_secrets\": {\n      \"type\": \"string\",\n      \"description\": \"The leve of permission to grant the access token to manage Dependabot secrets.\"\
  ,\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"deployments\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for deployments and deployment statuses.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"environments\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for managing repository environments.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"issues\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for issues and related comments, assignees, labels, and milestones.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"metadata\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The level of permission to grant the access token to search repositories, list collaborators, and access repository metadata.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"packages\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for packages published to GitHub Packages.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"pages\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to retrieve Pages statuses, configuration, and builds, as well as create new builds.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"pull_requests\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for pull requests\
  \ and related comments, assignees, labels, milestones, and merges.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"repository_hooks\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage the post-receive hooks for a repository.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"repository_projects\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage repository projects, columns, and cards.\",\n      \"enum\": [\n        \"read\",\n        \"write\",\n        \"admin\"\n      ],\n      \"example\": \"read\"\n    },\n    \"secret_scanning_alerts\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage secret scanning alerts.\",\n      \"enum\": [\n        \"read\"\
  ,\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"secrets\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage repository secrets.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"security_events\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage security events like code scanning alerts.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"single_file\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage just a single file.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"statuses\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to\
  \ grant the access token for commit statuses.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ],\n      \"example\": \"read\"\n    },\n    \"vulnerability_alerts\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage Dependabot alerts.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"workflows\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to update GitHub Actions workflow files.\",\n      \"enum\": [\n        \"write\"\n      ]\n    },\n    \"members\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for organization teams and members.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_administration\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access\
  \ token to manage access to an organization.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_custom_roles\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for custom repository roles management.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_copilot_seat_management\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for managing access to GitHub Copilot for members of an organization with a Copilot Business subscription. This property is in beta and is subject to change.\",\n      \"enum\": [\n        \"write\"\n      ]\n    },\n    \"organization_announcement_banners\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage announcement banners for an organization.\",\n      \"enum\": [\n        \"read\"\
  ,\n        \"write\"\n      ]\n    },\n    \"organization_events\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view events triggered by an activity in an organization.\",\n      \"enum\": [\n        \"read\"\n      ]\n    },\n    \"organization_hooks\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage the post-receive hooks for an organization.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_personal_access_tokens\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for viewing and managing fine-grained personal access token requests to an organization.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_personal_access_token_requests\": {\n      \"type\": \"string\",\n      \"description\": \"The level of\
  \ permission to grant the access token for viewing and managing fine-grained personal access tokens that have been approved by an organization.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_plan\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for viewing an organization's plan.\",\n      \"enum\": [\n        \"read\"\n      ]\n    },\n    \"organization_projects\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage organization projects and projects beta (where available).\",\n      \"enum\": [\n        \"read\",\n        \"write\",\n        \"admin\"\n      ]\n    },\n    \"organization_packages\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token for organization packages published to GitHub Packages.\",\n      \"enum\": [\n        \"read\",\n        \"\
  write\"\n      ]\n    },\n    \"organization_secrets\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage organization secrets.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_self_hosted_runners\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage GitHub Actions self-hosted runners available to an organization.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"organization_user_blocking\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage users blocked by the organization.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"team_discussions\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage\
  \ team discussions and related comments.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"email_addresses\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage the email addresses belonging to a user.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"followers\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage the followers belonging to a user.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"git_ssh_keys\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage git SSH keys.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"gpg_keys\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage\
  \ GPG keys belonging to a user.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"interaction_limits\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to view and manage interaction limits on a repository.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to manage the profile settings belonging to a user.\",\n      \"enum\": [\n        \"write\"\n      ]\n    },\n    \"starring\": {\n      \"type\": \"string\",\n      \"description\": \"The level of permission to grant the access token to list and manage repositories a user is starring.\",\n      \"enum\": [\n        \"read\",\n        \"write\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-app-permissions-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: app-permissions
---
