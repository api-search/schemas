---
description: Minimal reference to a Basecamp person
layout: schema
name: PersonRef
properties_list:
- description: Person ID
  name: id
  type: integer
- description: Signed global ID for attaching this person
  name: attachable_sgid
  type: string
- description: Full name
  name: name
  type: string
- description: Email address
  name: email_address
  type: string
- description: Type of personable (User, Client, etc.)
  name: personable_type
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
- description: Account creation timestamp
  name: created_at
  type: string
- description: Last update timestamp
  name: updated_at
  type: string
- description: Whether the person is an account administrator
  name: admin
  type: boolean
- description: Whether the person is the account owner
  name: owner
  type: boolean
- description: Whether the person is a client user
  name: client
  type: boolean
- description: Whether the person is an employee
  name: employee
  type: boolean
- description: IANA time zone name
  name: time_zone
  type: string
- description: URL to the person's avatar image
  name: avatar_url
  type: string
- description: Company the person belongs to
  name: company
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/personref-schema.json
slug: personref
source_filename: personref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/personref-schema.json\",\n  \"title\": \"PersonRef\",\n  \"type\": \"object\",\n  \"description\": \"Minimal reference to a Basecamp person\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Person ID\"\n    },\n    \"attachable_sgid\": {\n      \"type\": \"string\",\n      \"description\": \"Signed global ID for attaching this person\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name\"\n    },\n    \"email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address\"\n    },\n    \"personable_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of personable (User, Client, etc.)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title\"\n    },\n    \"\
  bio\": {\n      \"type\": \"string\",\n      \"description\": \"Short biography\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Location string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account creation timestamp\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person is an account administrator\"\n    },\n    \"owner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person is the account owner\"\n    },\n    \"client\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person is a client user\"\n    },\n    \"employee\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person is an employee\"\n    },\n    \"time_zone\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"IANA time zone name\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the person's avatar image\"\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"description\": \"Company the person belongs to\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Company ID\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Company name\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/personref-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: PersonRef
---
