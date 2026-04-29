---
description: A member of a core facility.
layout: schema
name: Member
properties_list:
- description: Unique identifier for the member.
  name: id
  type: integer
- description: Full name of the member.
  name: name
  type: string
- description: Email address of the member.
  name: email
  type: string
- description: Role of the member in the core.
  name: role
  type: string
- description: Membership status.
  name: status
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-member-schema.json
slug: ilab-operations-api-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"A member of a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the member.\",\n      \"example\": 400111\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the member.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the member.\",\n      \"example\": \"jsmith@stanford.edu\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role of the member in the core.\",\n      \"enum\": [\n        \"pi\",\n        \"researcher\"\
  ,\n        \"admin\",\n        \"staff\"\n      ],\n      \"example\": \"pi\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Membership status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-member-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Member
---
