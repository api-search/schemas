---
description: A cloud rule enforces policies on cloud accounts by bundling IAM policies, CloudFormation templates, Azure ARM templates, compliance standards, and other governance artifacts.
layout: schema
name: Kion Cloud Rule
properties_list:
- description: Internal Kion cloud rule ID.
  name: id
  type: integer
- description: Cloud rule name.
  name: name
  type: string
- description: Cloud rule description.
  name: description
  type: string
- description: Webhook ID to trigger before rule application.
  name: pre_webhook_id
  type: integer
- description: Webhook ID to trigger after rule application.
  name: post_webhook_id
  type: integer
- description: Whether this is a built-in cloud rule.
  name: built_in
  type: boolean
- description: Owner users of the cloud rule.
  name: owner_users
  type: array
- description: Owner user groups of the cloud rule.
  name: owner_user_groups
  type: array
- description: AWS IAM policy IDs attached to the rule.
  name: aws_iam_policies
  type: array
- description: CloudFormation template IDs attached to the rule.
  name: aws_cloudformation_templates
  type: array
- description: Azure ARM template IDs attached to the rule.
  name: azure_arm_template_definitions
  type: array
- description: Azure policy IDs attached to the rule.
  name: azure_policy_definitions
  type: array
- description: Azure role IDs attached to the rule.
  name: azure_role_definitions
  type: array
- description: Compliance standard IDs attached to the rule.
  name: compliance_standards
  type: array
- description: GCP IAM role IDs attached to the rule.
  name: gcp_iam_roles
  type: array
- description: Service control policy IDs attached to the rule.
  name: service_control_policies
  type: array
- description: OU IDs the rule is applied to.
  name: ous
  type: array
- description: Project IDs the rule is applied to.
  name: projects
  type: array
- description: Labels associated with the cloud rule.
  name: labels
  type: object
- description: Timestamp when the cloud rule was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/cloud-rule.json
slug: cloud-rule
source_filename: cloud-rule.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/cloud-rule.json\",\n  \"title\": \"Kion Cloud Rule\",\n  \"description\": \"A cloud rule enforces policies on cloud accounts by bundling IAM policies, CloudFormation templates, Azure ARM templates, compliance standards, and other governance artifacts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion cloud rule ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud rule name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud rule description.\"\n    },\n    \"pre_webhook_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Webhook ID to trigger before rule application.\"\n    },\n    \"post_webhook_id\": {\n      \"type\": \"integer\",\n      \"description\":\
  \ \"Webhook ID to trigger after rule application.\"\n    },\n    \"built_in\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a built-in cloud rule.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the cloud rule.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the cloud rule.\"\n    },\n    \"aws_iam_policies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"AWS IAM policy IDs attached to the rule.\"\n    },\n    \"aws_cloudformation_templates\": {\n      \"type\": \"array\",\n      \"items\": { \"type\"\
  : \"integer\" },\n      \"description\": \"CloudFormation template IDs attached to the rule.\"\n    },\n    \"azure_arm_template_definitions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Azure ARM template IDs attached to the rule.\"\n    },\n    \"azure_policy_definitions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Azure policy IDs attached to the rule.\"\n    },\n    \"azure_role_definitions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Azure role IDs attached to the rule.\"\n    },\n    \"compliance_standards\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Compliance standard IDs attached to the rule.\"\n    },\n    \"gcp_iam_roles\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"GCP IAM role IDs attached\
  \ to the rule.\"\n    },\n    \"service_control_policies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Service control policy IDs attached to the rule.\"\n    },\n    \"ous\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"OU IDs the rule is applied to.\"\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"Project IDs the rule is applied to.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the cloud rule.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cloud rule was created.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/cloud-rule.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Cloud Rule
---
