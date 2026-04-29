---
description: EligibilityList schema from Availity API
layout: schema
name: EligibilityList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-eligibility-list-schema.json
slug: eligibility-eligibility-list
source_filename: eligibility-eligibility-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-eligibility-list-schema.json\",\n  \"title\": \"EligibilityList\",\n  \"description\": \"EligibilityList schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EligibilityResponse\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-eligibility-list-schema.json
tags: []
title: EligibilityList
---
