---
description: An AWS IAM policy managed through Kion for applying identity and access management controls to cloud accounts.
layout: schema
name: Kion AWS IAM Policy
properties_list:
- description: Internal Kion policy ID.
  name: id
  type: integer
- description: Policy name.
  name: name
  type: string
- description: Policy description.
  name: description
  type: string
- description: IAM path for the policy.
  name: aws_iam_path
  type: string
- description: JSON policy document.
  name: policy
  type: string
- description: Whether this is an AWS managed policy.
  name: aws_managed_policy
  type: boolean
- description: Owner users of the policy.
  name: owner_users
  type: array
- description: Owner user groups of the policy.
  name: owner_user_groups
  type: array
- description: Labels associated with the policy.
  name: labels
  type: object
- description: Timestamp when the policy was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/aws-iam-policy.json
slug: aws-iam-policy
source_filename: aws-iam-policy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/aws-iam-policy.json\",\n  \"title\": \"Kion AWS IAM Policy\",\n  \"description\": \"An AWS IAM policy managed through Kion for applying identity and access management controls to cloud accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion policy ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Policy description.\"\n    },\n    \"aws_iam_path\": {\n      \"type\": \"string\",\n      \"description\": \"IAM path for the policy.\"\n    },\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"JSON policy document.\"\n    },\n    \"aws_managed_policy\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether this is an AWS managed policy.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the policy.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the policy.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the policy.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the policy was created.\"\n    }\n  },\n  \"required\": [\"name\", \"policy\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/aws-iam-policy.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion AWS IAM Policy
---
