---
description: A user within an Intralinks workspace who is assigned a role and belongs to one or more groups for document access control.
layout: schema
name: Intralinks User
properties_list:
- description: Unique identifier of the user.
  name: id
  type: string
- description: First name.
  name: firstName
  type: string
- description: Last name.
  name: lastName
  type: string
- description: Email address.
  name: emailId
  type: string
- description: Organization name.
  name: organization
  type: string
- description: Role assigned to the user in the workspace.
  name: roleType
  type: string
- description: Timestamp of last workspace access.
  name: lastAccessedOn
  type: string
- description: User creation timestamp.
  name: createdOn
  type: string
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"user.json\",\n  \"title\": \"Intralinks User\",\n  \"description\": \"A user within an Intralinks workspace who is assigned a role and belongs to one or more groups for document access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the user.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\"\n    },\n    \"emailId\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\"\n    },\n    \"organization\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name.\"\n    },\n    \"roleType\": {\n      \"type\": \"string\",\n      \"description\": \"Role assigned to the user in the workspace.\"\
  \n    },\n    \"lastAccessedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last workspace access.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"User creation timestamp.\"\n    }\n  },\n  \"required\": [\"emailId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/user.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks User
---
