---
description: A project in Helix Swarm, grouping branches, members, and review settings.
layout: schema
name: Project
properties_list:
- description: The project identifier.
  name: id
  type: string
- description: The project display name.
  name: name
  type: string
- description: The project description.
  name: description
  type: string
- description: List of project member usernames.
  name: members
  type: array
- description: List of project owner usernames.
  name: owners
  type: array
- description: List of associated Perforce groups.
  name: subgroups
  type: array
- description: Branch definitions for the project.
  name: branches
  type: array
- description: Whether the project has been deleted.
  name: deleted
  type: boolean
- description: Deploy configuration for the project.
  name: deploy
  type: object
- description: Email notification settings.
  name: emailFlags
  type: object
- description: A Perforce jobview expression for the project.
  name: jobview
  type: string
- description: Minimum number of up votes required for approval.
  name: minimumUpVotes
  type: integer
- description: Whether the project is private.
  name: private
  type: boolean
- description: Whether to retain default reviewers on review updates.
  name: retainDefaultReviewers
  type: boolean
- description: Test configuration for the project.
  name: tests
  type: object
- description: The workflow identifier associated with the project.
  name: workflow
  type: string
- description: Default settings for the project.
  name: defaults
  type: object
- description: The project readme content.
  name: readme
  type: string
provider_name: Perforce
provider_slug: perforce
schema_file: json-schema/perforce-helix-swarm-project-schema.json
slug: perforce-helix-swarm-project
source_filename: perforce-helix-swarm-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"description\": \"A project in Helix Swarm, grouping branches, members, and review settings.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The project identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The project display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The project description.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"List of project member usernames.\"\n    },\n    \"owners\": {\n      \"type\": \"array\",\n      \"description\": \"List of project owner usernames.\"\n    },\n    \"subgroups\": {\n      \"type\": \"array\",\n      \"description\": \"List of associated Perforce groups.\"\n    },\n    \"branches\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Branch definitions for the project.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project has been deleted.\"\n    },\n    \"deploy\": {\n      \"type\": \"object\",\n      \"description\": \"Deploy configuration for the project.\"\n    },\n    \"emailFlags\": {\n      \"type\": \"object\",\n      \"description\": \"Email notification settings.\"\n    },\n    \"jobview\": {\n      \"type\": \"string\",\n      \"description\": \"A Perforce jobview expression for the project.\"\n    },\n    \"minimumUpVotes\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of up votes required for approval.\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is private.\"\n    },\n    \"retainDefaultReviewers\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to retain default reviewers on review updates.\"\n    },\n    \"tests\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Test configuration for the project.\"\n    },\n    \"workflow\": {\n      \"type\": \"string\",\n      \"description\": \"The workflow identifier associated with the project.\"\n    },\n    \"defaults\": {\n      \"type\": \"object\",\n      \"description\": \"Default settings for the project.\"\n    },\n    \"readme\": {\n      \"type\": \"string\",\n      \"description\": \"The project readme content.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/json-schema/perforce-helix-swarm-project-schema.json
tags: []
title: Project
---
