---
description: ''
layout: schema
name: OrganizationAssignment
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: Whether this is the primary organization assignment.
  name: isPrimary
  type: boolean
provider_name: Workday
provider_slug: workday
schema_file: json-schema/staffing-organization-assignment-schema.json
slug: staffing-organization-assignment
source_filename: staffing-organization-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrganizationAssignment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"isPrimary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary organization assignment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/staffing-organization-assignment-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: OrganizationAssignment
---
