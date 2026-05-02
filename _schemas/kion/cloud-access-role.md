---
description: A cloud access role defines access permissions for users and groups to cloud accounts at the OU or project level, supporting AWS, Azure, and GCP IAM policies.
layout: schema
name: Kion Cloud Access Role
properties_list:
- description: Internal Kion cloud access role ID.
  name: id
  type: integer
- description: Cloud access role name.
  name: name
  type: string
- description: AWS IAM role name.
  name: aws_iam_role_name
  type: string
- description: Whether web console access is enabled.
  name: web_access
  type: boolean
- description: Whether short-term access keys are enabled.
  name: short_term_access_keys
  type: boolean
- description: Whether long-term access keys are enabled.
  name: long_term_access_keys
  type: boolean
- description: AWS IAM policy IDs attached to the role.
  name: aws_iam_policies
  type: array
- description: Azure role definition IDs attached to the role.
  name: azure_role_definitions
  type: array
- description: GCP IAM role IDs attached to the role.
  name: gcp_iam_roles
  type: array
- description: User IDs assigned to the role.
  name: users
  type: array
- description: User group IDs assigned to the role.
  name: user_groups
  type: array
- description: Account IDs the role applies to.
  name: accounts
  type: array
- description: Labels associated with the cloud access role.
  name: labels
  type: object
- description: Timestamp when the cloud access role was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/cloud-access-role.json
slug: cloud-access-role
source_filename: cloud-access-role.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/cloud-access-role.json\",\n  \"title\": \"Kion Cloud Access Role\",\n  \"description\": \"A cloud access role defines access permissions for users and groups to cloud accounts at the OU or project level, supporting AWS, Azure, and GCP IAM policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion cloud access role ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud access role name.\"\n    },\n    \"aws_iam_role_name\": {\n      \"type\": \"string\",\n      \"description\": \"AWS IAM role name.\"\n    },\n    \"web_access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether web console access is enabled.\"\n    },\n    \"short_term_access_keys\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether short-term access keys are enabled.\"\n    },\n    \"long_term_access_keys\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether long-term access keys are enabled.\"\n    },\n    \"aws_iam_policies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"AWS IAM policy IDs attached to the role.\"\n    },\n    \"azure_role_definitions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Azure role definition IDs attached to the role.\"\n    },\n    \"gcp_iam_roles\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"GCP IAM role IDs attached to the role.\"\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"User IDs assigned to the role.\"\n    },\n    \"user_groups\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n\
  \      \"description\": \"User group IDs assigned to the role.\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Account IDs the role applies to.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the cloud access role.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cloud access role was created.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/cloud-access-role.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Cloud Access Role
---
