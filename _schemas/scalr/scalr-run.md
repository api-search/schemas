---
description: A Scalr run representing a single Terraform plan and/or apply execution
layout: schema
name: Scalr Run
properties_list:
- description: Unique run identifier
  name: id
  type: string
- description: Current run status
  name: status
  type: string
- description: Parent workspace reference
  name: workspace
  type: object
- description: Whether this is a plan-only run (no apply)
  name: plan_only
  type: boolean
- description: Whether this run destroys all managed infrastructure
  name: is_destroy
  type: boolean
- description: Human-readable description of why the run was triggered
  name: message
  type: string
- description: What triggered this run
  name: trigger_reason
  type: string
- description: Whether apply was automatically triggered after plan
  name: auto_apply
  type: boolean
- description: Plan execution details
  name: plan
  type: object
- description: Apply execution details
  name: apply
  type: object
- description: Cost estimation results
  name: cost_estimate
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Scalr
provider_slug: scalr
schema_file: json-schema/scalr-run-schema.json
slug: scalr-run
source_filename: scalr-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalr/main/json-schema/scalr-run-schema.json\",\n  \"title\": \"Scalr Run\",\n  \"description\": \"A Scalr run representing a single Terraform plan and/or apply execution\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\", \"workspace\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique run identifier\",\n      \"pattern\": \"^run-[a-zA-Z0-9]+$\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\", \"plan_queued\", \"planning\", \"planned\", \"cost_estimating\",\n        \"cost_estimated\", \"policy_checking\", \"policy_override\", \"policy_soft_failed\",\n        \"policy_checked\", \"confirmed\", \"apply_queued\", \"applying\", \"applied\",\n        \"discarded\", \"errored\", \"canceled\", \"force_canceled\"\n      ],\n      \"description\"\
  : \"Current run status\"\n    },\n    \"workspace\": {\n      \"type\": \"object\",\n      \"description\": \"Parent workspace reference\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"plan_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a plan-only run (no apply)\"\n    },\n    \"is_destroy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this run destroys all managed infrastructure\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of why the run was triggered\"\n    },\n    \"trigger_reason\": {\n      \"type\": \"string\",\n      \"enum\": [\"manual\", \"vcs\", \"api\", \"schedule\"],\n      \"description\": \"What triggered this run\"\n    },\n    \"auto_apply\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether apply was automatically triggered after plan\"\n    },\n    \"plan\": {\n  \
  \    \"type\": \"object\",\n      \"description\": \"Plan execution details\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        },\n        \"resource_additions\": {\n          \"type\": \"integer\"\n        },\n        \"resource_changes\": {\n          \"type\": \"integer\"\n        },\n        \"resource_destructions\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"apply\": {\n      \"type\": \"object\",\n      \"description\": \"Apply execution details\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"cost_estimate\": {\n      \"type\": \"object\",\n      \"description\": \"Cost estimation results\",\n      \"properties\": {\n        \"proposed_monthly_cost\": {\n          \"type\": \"string\"\n        },\n        \"prior_monthly_cost\"\
  : {\n          \"type\": \"string\"\n        },\n        \"delta_monthly_cost\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalr/refs/heads/main/json-schema/scalr-run-schema.json
tags:
- FinOps
- GitOps
- Infrastructure as Code
- Kubernetes
- OPA
- OpenTofu
- Policy
- Terraform
title: Scalr Run
---
