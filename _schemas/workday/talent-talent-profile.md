---
description: ''
layout: schema
name: TalentProfile
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: jobHistory
  type: array
- description: ''
  name: education
  type: array
- description: ''
  name: skills
  type: array
- description: ''
  name: certifications
  type: array
- description: ''
  name: languages
  type: array
- description: ''
  name: careerInterests
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/talent-talent-profile-schema.json
slug: talent-talent-profile
source_filename: talent-talent-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TalentProfile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"jobHistory\": {\n      \"type\": \"array\"\n    },\n    \"education\": {\n      \"type\": \"array\"\n    },\n    \"skills\": {\n      \"type\": \"array\"\n    },\n    \"certifications\": {\n      \"type\": \"array\"\n    },\n    \"languages\": {\n      \"type\": \"array\"\n    },\n    \"careerInterests\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/talent-talent-profile-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TalentProfile
---
