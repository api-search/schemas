---
description: webhook-branch-protection-rule-created from GitHub API
layout: schema
name: webhook-branch-protection-rule-created
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: enterprise
  type: object
- description: ''
  name: installation
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: repository
  type: object
- description: The branch protection rule. Includes a `name` and all the [branch protection settings](https://docs.github.com/enterprise-server@3.9/github/administering-a-repository/defining-the-mergeability-of-pull
  name: rule
  type: object
- description: ''
  name: sender
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-emojis-webhook-branch-protection-rule-created-schema.json
slug: github-emojis-webhook-branch-protection-rule-created
source_filename: github-emojis-webhook-branch-protection-rule-created-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-emojis-webhook-branch-protection-rule-created-schema.json\",\n  \"title\": \"webhook-branch-protection-rule-created\",\n  \"description\": \"webhook-branch-protection-rule-created from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"created\"\n      ],\n      \"example\": \"created\"\n    },\n    \"enterprise\": {\n      \"$ref\": \"#/components/schemas/enterprise-webhooks\"\n    },\n    \"installation\": {\n      \"$ref\": \"#/components/schemas/simple-installation\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/organization-simple-webhooks\"\n    },\n    \"repository\": {\n      \"$ref\": \"#/components/schemas/repository-webhooks\"\n    },\n    \"rule\": {\n      \"title\": \"branch protection\
  \ rule\",\n      \"description\": \"The branch protection rule. Includes a `name` and all the [branch protection settings](https://docs.github.com/enterprise-server@3.9/github/administering-a-repository/defining-the-mergeability-of-pull-requests/about-protected-branches#about-branch-protection-settings) applied to branches that match the name. Binary settings are boolean. Multi-level configurations are one of `off`, `non_admins`, or `everyone`. Actor and build lists are arrays of strings.\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"admin_enforced\": {\n          \"type\": \"boolean\"\n        },\n        \"allow_deletions_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"allow_force_pushes_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n   \
  \         \"everyone\"\n          ]\n        },\n        \"authorized_actor_names\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"authorized_actors_only\": {\n          \"type\": \"boolean\"\n        },\n        \"authorized_dismissal_actors_only\": {\n          \"type\": \"boolean\"\n        },\n        \"create_protected\": {\n          \"type\": \"boolean\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"dismiss_stale_reviews_on_push\": {\n          \"type\": \"boolean\"\n        },\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"ignore_approvals_from_contributors\": {\n          \"type\": \"boolean\"\n        },\n        \"linear_history_requirement_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"\
  everyone\"\n          ]\n        },\n        \"merge_queue_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"pull_request_reviews_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"repository_id\": {\n          \"type\": \"integer\"\n        },\n        \"require_code_owner_review\": {\n          \"type\": \"boolean\"\n        },\n        \"required_approving_review_count\": {\n          \"type\": \"integer\"\n        },\n        \"required_conversation_resolution_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"required_deployments_enforcement_level\"\
  : {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"required_status_checks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"required_status_checks_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"signature_requirement_enforcement_level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"off\",\n            \"non_admins\",\n            \"everyone\"\n          ]\n        },\n        \"strict_required_status_checks_policy\": {\n          \"type\": \"boolean\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      },\n      \"required\": [\n        \"id\"\
  ,\n        \"repository_id\",\n        \"name\",\n        \"created_at\",\n        \"updated_at\",\n        \"pull_request_reviews_enforcement_level\",\n        \"required_approving_review_count\",\n        \"dismiss_stale_reviews_on_push\",\n        \"require_code_owner_review\",\n        \"authorized_dismissal_actors_only\",\n        \"ignore_approvals_from_contributors\",\n        \"required_status_checks\",\n        \"required_status_checks_enforcement_level\",\n        \"strict_required_status_checks_policy\",\n        \"signature_requirement_enforcement_level\",\n        \"linear_history_requirement_enforcement_level\",\n        \"admin_enforced\",\n        \"allow_force_pushes_enforcement_level\",\n        \"allow_deletions_enforcement_level\",\n        \"merge_queue_enforcement_level\",\n        \"required_deployments_enforcement_level\",\n        \"required_conversation_resolution_level\",\n        \"authorized_actors_only\",\n        \"authorized_actor_names\"\n      ]\n    },\n\
  \    \"sender\": {\n      \"$ref\": \"#/components/schemas/simple-user-webhooks\"\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"rule\",\n    \"repository\",\n    \"sender\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-emojis-webhook-branch-protection-rule-created-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: webhook-branch-protection-rule-created
---
