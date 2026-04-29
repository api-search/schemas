---
description: ''
layout: schema
name: CompensationChangeRequest
properties_list:
- description: The effective date of the compensation change.
  name: effectiveDate
  type: string
- description: ''
  name: proposedCompensation
  type: object
provider_name: Workday
provider_slug: workday
schema_file: json-schema/compensation-compensation-change-request-schema.json
slug: compensation-compensation-change-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompensationChangeRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"The effective date of the compensation change.\"\n    },\n    \"proposedCompensation\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/compensation-compensation-change-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: CompensationChangeRequest
---
