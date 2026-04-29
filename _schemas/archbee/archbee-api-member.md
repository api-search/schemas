---
description: ''
layout: schema
name: Member
properties_list:
- description: User identifier
  name: id
  type: string
- description: Member email address
  name: email
  type: string
- description: Member display name
  name: name
  type: string
- description: Member role in the space
  name: role
  type: string
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-member-schema.json
slug: archbee-api-member
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier\",\n      \"example\": \"usr_abc123\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Member email address\",\n      \"example\": \"alice@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Member display name\",\n      \"example\": \"Alice Smith\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Member role in the space\",\n      \"enum\": [\n        \"owner\",\n        \"admin\",\n        \"editor\",\n        \"viewer\",\n        \"commenter\"\n      ],\n      \"example\": \"editor\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-member-schema.json\",\n  \"title\": \"\
  Member\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-member-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: Member
---
