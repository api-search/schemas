---
description: An employee leave allowance record for a specific reason type and year.
layout: schema
name: Allowance
properties_list:
- description: Unique identifier of the allowance.
  name: _id
  type: string
- description: ID of the user this allowance belongs to.
  name: userId
  type: string
- description: ID of the absence reason type this allowance is for.
  name: reasonId
  type: string
- description: Calendar year this allowance applies to.
  name: year
  type: integer
- description: Total number of days allowed.
  name: allowance
  type: number
- description: Number of days used.
  name: used
  type: number
- description: Number of days remaining.
  name: remaining
  type: number
- description: Number of days carried over from the previous year.
  name: carryover
  type: number
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/allowance-schema.json
slug: allowance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/allowance-schema.json\",\n  \"title\": \"Allowance\",\n  \"description\": \"An employee leave allowance record for a specific reason type and year.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the allowance.\",\n      \"example\": \"500234\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user this allowance belongs to.\",\n      \"example\": \"500456\"\n    },\n    \"reasonId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the absence reason type this allowance is for.\",\n      \"example\": \"500789\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Calendar year this allowance applies to.\",\n      \"example\": 2025\n\
  \    },\n    \"allowance\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of days allowed.\",\n      \"example\": 25\n    },\n    \"used\": {\n      \"type\": \"number\",\n      \"description\": \"Number of days used.\",\n      \"example\": 10\n    },\n    \"remaining\": {\n      \"type\": \"number\",\n      \"description\": \"Number of days remaining.\",\n      \"example\": 15\n    },\n    \"carryover\": {\n      \"type\": \"number\",\n      \"description\": \"Number of days carried over from the previous year.\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/allowance-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: Allowance
---
