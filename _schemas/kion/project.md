---
description: A project is the organizational unit for attaching cloud accounts, managing funding, and applying governance policies in Kion.
layout: schema
name: Kion Project
properties_list:
- description: Internal Kion project ID.
  name: id
  type: integer
- description: Project name.
  name: name
  type: string
- description: Project description.
  name: description
  type: string
- description: Organizational unit ID the project belongs to.
  name: ou_id
  type: integer
- description: Default AWS region for the project.
  name: default_aws_region
  type: string
- description: Permission scheme ID applied to the project.
  name: permission_scheme_id
  type: integer
- description: Funding allocations for the project.
  name: project_funding
  type: array
- description: Budget configuration for the project.
  name: budget
  type: object
- description: Labels associated with the project.
  name: labels
  type: object
- description: Whether the project is archived.
  name: archived
  type: boolean
- description: Whether auto-pay is enabled.
  name: auto_pay
  type: boolean
- description: Timestamp when the project was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/project.json
slug: project
source_filename: project.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/project.json\",\n  \"title\": \"Kion Project\",\n  \"description\": \"A project is the organizational unit for attaching cloud accounts, managing funding, and applying governance policies in Kion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion project ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Project name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Project description.\"\n    },\n    \"ou_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organizational unit ID the project belongs to.\"\n    },\n    \"default_aws_region\": {\n      \"type\": \"string\",\n      \"description\": \"Default AWS region for the project.\"\n    },\n    \"permission_scheme_id\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Permission scheme ID applied to the project.\"\n    },\n    \"project_funding\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"funding_source_id\": {\n            \"type\": \"integer\",\n            \"description\": \"Funding source ID.\"\n          },\n          \"amount\": {\n            \"type\": \"number\",\n            \"description\": \"Funding amount.\"\n          },\n          \"start_datecode\": {\n            \"type\": \"string\",\n            \"description\": \"Funding start date.\"\n          },\n          \"end_datecode\": {\n            \"type\": \"string\",\n            \"description\": \"Funding end date.\"\n          }\n        }\n      },\n      \"description\": \"Funding allocations for the project.\"\n    },\n    \"budget\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"number\"\
  ,\n          \"description\": \"Budget amount.\"\n        },\n        \"funding_source_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Funding source ID for the budget.\"\n        }\n      },\n      \"description\": \"Budget configuration for the project.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the project.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is archived.\"\n    },\n    \"auto_pay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether auto-pay is enabled.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was created.\"\n    }\n  },\n  \"required\": [\"name\", \"ou_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/project.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Project
---
