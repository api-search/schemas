---
description: A SAFe Program Increment (PI) representing a fixed timebox of 8-12 weeks for an Agile Release Train
layout: schema
name: SAFe Program Increment
properties_list:
- description: Unique PI identifier
  name: id
  type: string
- description: PI name (e.g., PI 2026.2)
  name: name
  type: string
- description: PI start date
  name: start_date
  type: string
- description: PI end date
  name: end_date
  type: string
- description: Agile Release Train this PI belongs to
  name: art
  type: object
- description: Current PI status
  name: status
  type: string
- description: Sprints/Iterations within this PI
  name: iterations
  type: array
- description: PI objectives committed by teams
  name: objectives
  type: array
- description: Features planned for this PI
  name: features
  type: array
provider_name: Scaled Agile
provider_slug: scaled-agile
schema_file: json-schema/scaled-agile-pi-schema.json
slug: scaled-agile-pi
source_filename: scaled-agile-pi-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scaled-agile/main/json-schema/scaled-agile-pi-schema.json\",\n  \"title\": \"SAFe Program Increment\",\n  \"description\": \"A SAFe Program Increment (PI) representing a fixed timebox of 8-12 weeks for an Agile Release Train\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"start_date\", \"end_date\", \"art\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique PI identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"PI name (e.g., PI 2026.2)\",\n      \"examples\": [\"PI 2026.1\", \"PI 2026.2\", \"PI Q2 FY26\"]\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"PI start date\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\"\
  : \"PI end date\"\n    },\n    \"art\": {\n      \"type\": \"object\",\n      \"description\": \"Agile Release Train this PI belongs to\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"planning\", \"active\", \"completed\"],\n      \"description\": \"Current PI status\"\n    },\n    \"iterations\": {\n      \"type\": \"array\",\n      \"description\": \"Sprints/Iterations within this PI\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"number\": {\n            \"type\": \"integer\",\n            \"description\": \"Iteration number within PI (1-5, where 5 is typically IP)\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"start_date\": {\n\
  \            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"end_date\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"development\", \"innovation_planning\"],\n            \"description\": \"Iteration type\"\n          }\n        }\n      }\n    },\n    \"objectives\": {\n      \"type\": \"array\",\n      \"description\": \"PI objectives committed by teams\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          },\n          \"business_value\": {\n            \"type\": \"integer\",\n            \"minimum\": 1,\n            \"maximum\": 10,\n            \"description\": \"Business value rating (1-10)\"\n          },\n          \"committed\": {\n            \"type\": \"boolean\"\
  \n          },\n          \"team\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"Features planned for this PI\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\"planned\", \"in_progress\", \"done\", \"accepted\"]\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scaled-agile/refs/heads/main/json-schema/scaled-agile-pi-schema.json
tags:
- Agile
- Business Agility
- DevOps
- Enterprise
- Lean
- Project Management
- SAFe
- Scaled Agile
title: SAFe Program Increment
---
