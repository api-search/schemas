---
description: Permit schema from Adyen API
layout: schema
name: Permit
properties_list:
- description: Partner ID (when using the permit-per-partner token sharing model).
  name: partnerId
  type: string
- description: The profile to apply to this permit (when using the shared permits model).
  name: profileReference
  type: string
- description: Permit level restriction overrides.
  name: restriction
  type: object
- description: The key to link permit requests to permit results.
  name: resultKey
  type: string
- description: The expiry date for this permit.
  name: validTillDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-permit-schema.json
slug: recurring-permit
source_filename: recurring-permit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-permit-schema.json\",\n  \"title\": \"Permit\",\n  \"description\": \"Permit schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partnerId\": {\n      \"description\": \"Partner ID (when using the permit-per-partner token sharing model).\",\n      \"type\": \"string\"\n    },\n    \"profileReference\": {\n      \"description\": \"The profile to apply to this permit (when using the shared permits model).\",\n      \"type\": \"string\"\n    },\n    \"restriction\": {\n      \"description\": \"Permit level restriction overrides.\",\n      \"$ref\": \"#/components/schemas/PermitRestriction\"\n    },\n    \"resultKey\": {\n      \"description\": \"The key to link permit requests to permit results.\",\n      \"type\": \"string\"\n    },\n    \"validTillDate\": {\n      \"description\"\
  : \"The expiry date for this permit.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-permit-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Permit
---
