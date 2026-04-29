---
description: An Air Force Reserve career opportunity
layout: schema
name: CareerOpportunity
properties_list:
- description: Air Force Specialty Code
  name: afsc_code
  type: string
- description: Career field title
  name: title
  type: string
- description: Career field description
  name: description
  type: string
- description: Career category
  name: category
  type: string
- description: Minimum entry rank/grade
  name: minimum_grade
  type: string
- description: Enlistment bonus available
  name: enlistment_bonus
  type: boolean
provider_name: Air Force Reserve
provider_slug: air-force-reserve
schema_file: json-schema/afrc-career-opportunity-schema.json
slug: afrc-career-opportunity
source_filename: afrc-career-opportunity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/json-schema/afrc-career-opportunity-schema.json\",\n  \"title\": \"CareerOpportunity\",\n  \"description\": \"An Air Force Reserve career opportunity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"afsc_code\": {\n      \"type\": \"string\",\n      \"description\": \"Air Force Specialty Code\",\n      \"example\": \"17DX\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Career field title\",\n      \"example\": \"Cyber Warfare Operations\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Career field description\",\n      \"example\": \"Conducts offensive and defensive cyberspace operations\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Career category\",\n      \"example\": \"Cyber\"\n    },\n \
  \   \"minimum_grade\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum entry rank/grade\",\n      \"example\": \"E-1\"\n    },\n    \"enlistment_bonus\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enlistment bonus available\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/json-schema/afrc-career-opportunity-schema.json
tags:
- Federal Government
- Military
- Defense
- Air Force
- United States Government
title: CareerOpportunity
---
