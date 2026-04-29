---
description: Schema for an Apache Software Foundation Project Management Committee (PMC) as returned by the Projects and Whimsy APIs.
layout: schema
name: Apache Software Foundation Committee
properties_list:
- description: The committee display name
  name: name
  type: string
- description: Apache ID of the committee chair
  name: chair
  type: string
- description: A brief description of the committee
  name: description
  type: string
- description: The committee homepage URL
  name: homepage
  type: string
- description: Date the committee was established (e.g., 2002-01)
  name: established
  type: string
- description: Whether this is a Project Management Committee
  name: pmc
  type: boolean
- description: Reporting schedule months (e.g., ['January', 'April', 'July', 'October'])
  name: report
  type: array
- description: Committee roster keyed by Apache ID
  name: roster
  type: object
- description: Number of members in the committee roster
  name: roster_count
  type: integer
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
schema_file: json-schema/apache-software-foundation-committee-schema.json
slug: apache-software-foundation-committee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"apache-software-foundation-committee-schema.json\",\n  \"title\": \"Apache Software Foundation Committee\",\n  \"description\": \"Schema for an Apache Software Foundation Project Management Committee (PMC) as returned by the Projects and Whimsy APIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The committee display name\"\n    },\n    \"chair\": {\n      \"type\": \"string\",\n      \"description\": \"Apache ID of the committee chair\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the committee\"\n    },\n    \"homepage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The committee homepage URL\"\n    },\n    \"established\": {\n      \"type\": \"string\",\n      \"description\": \"Date the committee was established\
  \ (e.g., 2002-01)\"\n    },\n    \"pmc\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a Project Management Committee\"\n    },\n    \"report\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Reporting schedule months (e.g., ['January', 'April', 'July', 'October'])\"\n    },\n    \"roster\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the member\"\n          },\n          \"date\": {\n            \"type\": \"string\",\n            \"description\": \"Date the member joined the committee\"\n          }\n        }\n      },\n      \"description\": \"Committee roster keyed by Apache ID\"\n    },\n    \"roster_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members in the committee roster\"\
  \n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/json-schema/apache-software-foundation-committee-schema.json
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
title: Apache Software Foundation Committee
---
