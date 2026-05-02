---
description: A compliance check defines an automated audit rule for verifying cloud resource configurations against organizational policies.
layout: schema
name: Kion Compliance Check
properties_list:
- description: Internal Kion compliance check ID.
  name: id
  type: integer
- description: Compliance check name.
  name: name
  type: string
- description: Compliance check description.
  name: description
  type: string
- description: Cloud provider ID this check applies to.
  name: cloud_provider_id
  type: integer
- description: Type of compliance check.
  name: compliance_check_type_id
  type: integer
- description: Severity level of the check.
  name: severity_type_id
  type: integer
- description: The compliance check policy body.
  name: body
  type: string
- description: How often the check runs in minutes.
  name: frequency_minutes
  type: integer
- description: Frequency type identifier.
  name: frequency_type_id
  type: integer
- description: Whether the check applies to all regions.
  name: is_all_regions
  type: boolean
- description: Whether findings are auto-archived.
  name: is_auto_archived
  type: boolean
- description: Specific regions to run the check in.
  name: regions
  type: array
- description: Owner users of the compliance check.
  name: owner_users
  type: array
- description: Owner user groups of the compliance check.
  name: owner_user_groups
  type: array
- description: Labels associated with the compliance check.
  name: labels
  type: object
- description: Timestamp when the compliance check was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/compliance-check.json
slug: compliance-check
source_filename: compliance-check.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/compliance-check.json\",\n  \"title\": \"Kion Compliance Check\",\n  \"description\": \"A compliance check defines an automated audit rule for verifying cloud resource configurations against organizational policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion compliance check ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance check name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance check description.\"\n    },\n    \"cloud_provider_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Cloud provider ID this check applies to.\"\n    },\n    \"compliance_check_type_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Type of compliance\
  \ check.\"\n    },\n    \"severity_type_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Severity level of the check.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The compliance check policy body.\"\n    },\n    \"frequency_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"How often the check runs in minutes.\"\n    },\n    \"frequency_type_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Frequency type identifier.\"\n    },\n    \"is_all_regions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the check applies to all regions.\"\n    },\n    \"is_auto_archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether findings are auto-archived.\"\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Specific regions to run the check in.\"\n    },\n    \"owner_users\": {\n      \"type\": \"array\",\n\
  \      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner users of the compliance check.\"\n    },\n    \"owner_user_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" }\n        }\n      },\n      \"description\": \"Owner user groups of the compliance check.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the compliance check.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the compliance check was created.\"\n    }\n  },\n  \"required\": [\"name\", \"cloud_provider_id\", \"compliance_check_type_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/compliance-check.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Compliance Check
---
