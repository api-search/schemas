---
description: A skill record in the employee skills matrix
layout: schema
name: SkillRecord
properties_list:
- description: Unique skill identifier
  name: skillId
  type: string
- description: Skill name
  name: name
  type: string
- description: Whether this skill is required for the role
  name: required
  type: boolean
- description: Whether the employee has completed this skill
  name: completed
  type: boolean
- description: When the skill was completed
  name: completedAt
  type: string
- description: Score achieved (0-100)
  name: score
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-skill-record-schema.json
slug: acadia-skill-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-skill-record-schema.json\",\n  \"title\": \"SkillRecord\",\n  \"description\": \"A skill record in the employee skills matrix\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"skillId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique skill identifier\",\n      \"example\": \"skill-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Skill name\",\n      \"example\": \"Machine Startup\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this skill is required for the role\",\n      \"example\": true\n    },\n    \"completed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the employee has completed this skill\",\n      \"example\": true\n    },\n    \"completedAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"When the skill was completed\",\n      \"example\": \"2026-02-10T08:00:00Z\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"Score achieved (0-100)\",\n      \"example\": 95\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-skill-record-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: SkillRecord
---
