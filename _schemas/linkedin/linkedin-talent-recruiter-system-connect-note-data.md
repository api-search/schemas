---
description: NoteData from LinkedIn API
layout: schema
name: NoteData
properties_list:
- description: ''
  name: note
  type: string
- description: ''
  name: author
  type: object
- description: ''
  name: atsCreatedAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-note-data-schema.json
slug: linkedin-talent-recruiter-system-connect-note-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-note-data-schema.json\",\n  \"title\": \"NoteData\",\n  \"description\": \"NoteData from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"note\": {\n      \"type\": \"string\",\n      \"example\": \"Great candidate, recommend for next round.\"\n    },\n    \"author\": {\n      \"$ref\": \"#/components/schemas/PersonName\"\n    },\n    \"atsCreatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1702693664000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-note-data-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: NoteData
---
