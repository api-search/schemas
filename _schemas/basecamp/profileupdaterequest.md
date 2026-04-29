---
description: ''
layout: schema
name: ProfileUpdateRequest
properties_list:
- description: Full name
  name: name
  type: string
- description: Email address
  name: email_address
  type: string
- description: Job title
  name: title
  type: string
- description: Short biography
  name: bio
  type: string
- description: Location string
  name: location
  type: string
- description: IANA time zone name
  name: time_zone_name
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/profileupdaterequest-schema.json
slug: profileupdaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/profileupdaterequest-schema.json\",\n  \"title\": \"ProfileUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name\"\n    },\n    \"email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title\"\n    },\n    \"bio\": {\n      \"type\": \"string\",\n      \"description\": \"Short biography\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Location string\"\n    },\n    \"time_zone_name\": {\n      \"type\": \"string\",\n      \"description\": \"IANA time zone name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/profileupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProfileUpdateRequest
---
