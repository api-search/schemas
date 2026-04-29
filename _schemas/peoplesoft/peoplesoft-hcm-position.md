---
description: PeopleSoft HCM position data.
layout: schema
name: Position
properties_list:
- description: Position number.
  name: POSITION_NBR
  type: string
- description: Position description.
  name: DESCR
  type: string
- description: Department ID.
  name: DEPTID
  type: string
- description: Job code.
  name: JOBCODE
  type: string
- description: Location code.
  name: LOCATION
  type: string
- description: Reports-to position.
  name: REPORTS_TO
  type: string
- description: Maximum headcount.
  name: MAX_HEAD_COUNT
  type: integer
- description: Position status.
  name: POSN_STATUS
  type: string
- description: Effective date.
  name: EFFDT
  type: string
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-hcm-position-schema.json
slug: peoplesoft-hcm-position
source_filename: peoplesoft-hcm-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-hcm-position-schema.json\",\n  \"title\": \"Position\",\n  \"description\": \"PeopleSoft HCM position data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"POSITION_NBR\": {\n      \"type\": \"string\",\n      \"description\": \"Position number.\",\n      \"example\": \"00012345\"\n    },\n    \"DESCR\": {\n      \"type\": \"string\",\n      \"description\": \"Position description.\",\n      \"example\": \"Senior Software Engineer\"\n    },\n    \"DEPTID\": {\n      \"type\": \"string\",\n      \"description\": \"Department ID.\",\n      \"example\": \"10200\"\n    },\n    \"JOBCODE\": {\n      \"type\": \"string\",\n      \"description\": \"Job code.\",\n      \"example\": \"MGR001\"\n    },\n    \"LOCATION\": {\n      \"type\": \"string\",\n      \"description\": \"Location code.\",\n \
  \     \"example\": \"HQ001\"\n    },\n    \"REPORTS_TO\": {\n      \"type\": \"string\",\n      \"description\": \"Reports-to position.\",\n      \"example\": \"00012340\"\n    },\n    \"MAX_HEAD_COUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum headcount.\",\n      \"example\": 1\n    },\n    \"POSN_STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"Position status.\",\n      \"enum\": [\n        \"A\",\n        \"I\",\n        \"F\"\n      ],\n      \"example\": \"A\"\n    },\n    \"EFFDT\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Effective date.\",\n      \"example\": \"2024-01-01\"\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-hcm-position-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: Position
---
