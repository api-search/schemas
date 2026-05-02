---
description: An AWS CloudFormation template managed through Kion for deploying infrastructure resources to cloud accounts.
layout: schema
name: Kion CloudFormation Template
properties_list:
- description: Internal Kion template ID.
  name: id
  type: integer
- description: Template name.
  name: name
  type: string
- description: Template description.
  name: description
  type: string
- description: URL to the CloudFormation template.
  name: template_url
  type: string
- description: Template body content.
  name: template_body
  type: string
- description: AWS region for deployment.
  name: region
  type: string
- description: SNS ARNs for notifications.
  name: sns_arns
  type: string
- description: Whether termination protection is enabled.
  name: terminate_protected
  type: boolean
- description: Owner users of the template.
  name: owner_users
  type: array
- description: Owner user groups of the template.
  name: owner_user_groups
  type: array
- description: Labels associated with the template.
  name: labels
  type: object
- description: Timestamp when the template was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/cloudformation-template.json
slug: cloudformation-template
source_filename: cloudformation-template.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/cloudformation-template.json\",\n  \"title\": \"Kion CloudFormation Template\",\n  \"description\": \"An AWS CloudFormation template managed through Kion for deploying infrastructure resources to cloud accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion template ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description.\"\n    },\n    \"template_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the CloudFormation template.\"\n    },\n    \"template_body\": {\n      \"type\": \"string\",\n      \"description\": \"Template body content.\"\n    },\n    \"region\": {\n      \"\
  type\": \"string\",\n      \"description\": \"AWS region for deployment.\"\n    },\n    \"sns_arns\": {\n      \"type\": \"string\",\n      \"description\": \"SNS ARNs for notifications.\"\n    },\n    \"terminate_protected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether termination protection is enabled.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the template.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the template.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n   \
  \   \"description\": \"Labels associated with the template.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the template was created.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/cloudformation-template.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion CloudFormation Template
---
