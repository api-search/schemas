---
description: A Scalr workspace representing a single Terraform/OpenTofu root module execution context with state, variables, and run configuration
layout: schema
name: Scalr Workspace
properties_list:
- description: Unique identifier of the workspace
  name: id
  type: string
- description: Workspace name
  name: name
  type: string
- description: Parent environment reference
  name: environment
  type: object
- description: Current workspace status
  name: status
  type: string
- description: Terraform or OpenTofu version to use
  name: terraform_version
  type: string
- description: Whether to automatically apply plans without manual confirmation
  name: auto_apply
  type: boolean
- description: Auto-queuing behavior when workspace is created or configured
  name: auto_queue_runs
  type: string
- description: How Terraform operations are executed
  name: execution_mode
  type: string
- description: VCS integration configuration
  name: vcs_provider
  type: object
- description: Tags for workspace organization and policy targeting
  name: tags
  type: array
- description: Whether remote operations are enabled
  name: operations
  type: boolean
- description: Whether cost estimation runs before apply
  name: cost_estimation_enabled
  type: boolean
- description: Whether a run is currently active
  name: has_active_run
  type: boolean
- description: Reference to the current active run
  name: current_run
  type: object
- description: Reference to the most recent run
  name: latest_run
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Scalr
provider_slug: scalr
schema_file: json-schema/scalr-workspace-schema.json
slug: scalr-workspace
source_filename: scalr-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalr/main/json-schema/scalr-workspace-schema.json\",\n  \"title\": \"Scalr Workspace\",\n  \"description\": \"A Scalr workspace representing a single Terraform/OpenTofu root module execution context with state, variables, and run configuration\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"environment\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workspace\",\n      \"pattern\": \"^ws-[a-zA-Z0-9]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workspace name\",\n      \"maxLength\": 255\n    },\n    \"environment\": {\n      \"type\": \"object\",\n      \"description\": \"Parent environment reference\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"pattern\": \"^env-[a-zA-Z0-9]+$\"\
  \n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\", \"Active_Execution\"],\n      \"description\": \"Current workspace status\"\n    },\n    \"terraform_version\": {\n      \"type\": \"string\",\n      \"description\": \"Terraform or OpenTofu version to use\",\n      \"examples\": [\"1.9.0\", \"1.8.0\"]\n    },\n    \"auto_apply\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically apply plans without manual confirmation\"\n    },\n    \"auto_queue_runs\": {\n      \"type\": \"string\",\n      \"enum\": [\"skip_first\", \"always\", \"never\"],\n      \"description\": \"Auto-queuing behavior when workspace is created or configured\"\n    },\n    \"execution_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"remote\", \"local\", \"agent\"],\n      \"description\": \"How Terraform operations are executed\"\n    },\n    \"vcs_provider\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"VCS integration configuration\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"repo\": {\n          \"type\": \"string\",\n          \"description\": \"Repository path (org/repo)\"\n        },\n        \"branch\": {\n          \"type\": \"string\",\n          \"description\": \"Default branch to trigger runs from\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Relative path within repo to the Terraform root module\"\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Tags for workspace organization and policy targeting\"\n    },\n    \"operations\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether remote operations are enabled\"\n    },\n    \"cost_estimation_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether cost estimation runs before apply\"\n    },\n    \"has_active_run\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a run is currently active\"\n    },\n    \"current_run\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the current active run\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"latest_run\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the most recent run\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalr/refs/heads/main/json-schema/scalr-workspace-schema.json
tags:
- FinOps
- GitOps
- Infrastructure as Code
- Kubernetes
- OPA
- OpenTofu
- Policy
- Terraform
title: Scalr Workspace
---
