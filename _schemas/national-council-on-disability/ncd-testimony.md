---
description: Congressional testimony submitted by the National Council on Disability on disability policy matters.
layout: schema
name: NCD Congressional Testimony
properties_list:
- description: Title of the testimony
  name: title
  type: string
- description: Date testimony was delivered
  name: date
  type: string
- description: Congressional committee before which testimony was delivered
  name: committee
  type: string
- description: Congressional chamber
  name: chamber
  type: string
- description: Subject matter of the testimony
  name: subject
  type: string
- description: Primary disability policy area addressed
  name: policyArea
  type: string
- description: URL to the full testimony document
  name: documentURL
  type: string
provider_name: National Council on Disability
provider_slug: national-council-on-disability
schema_file: json-schema/ncd-testimony-schema.json
slug: ncd-testimony
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ncd.gov/schemas/testimony\",\n  \"title\": \"NCD Congressional Testimony\",\n  \"description\": \"Congressional testimony submitted by the National Council on Disability on disability policy matters.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"title\",\n    \"date\",\n    \"committee\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the testimony\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date testimony was delivered\"\n    },\n    \"committee\": {\n      \"type\": \"string\",\n      \"description\": \"Congressional committee before which testimony was delivered\"\n    },\n    \"chamber\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Senate\",\n        \"House\",\n        \"Joint\"\n      ],\n      \"description\": \"Congressional\
  \ chamber\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Subject matter of the testimony\"\n    },\n    \"policyArea\": {\n      \"type\": \"string\",\n      \"description\": \"Primary disability policy area addressed\"\n    },\n    \"documentURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full testimony document\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/national-council-on-disability/refs/heads/main/json-schema/ncd-testimony-schema.json
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
title: NCD Congressional Testimony
---
