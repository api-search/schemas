---
description: Email/password credentials for a user
layout: schema
name: CredentialsEmail
properties_list:
- description: Email address
  name: email
  type: string
- description: Whether these credentials are disabled
  name: is_disabled
  type: boolean
- description: Timestamp of last login with these credentials
  name: logged_in_at
  type: string
- description: Timestamp when these credentials were created
  name: created_at
  type: string
- description: Relative URL
  name: url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-credentials-email-schema.json
slug: looker-credentials-email
source_filename: looker-credentials-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CredentialsEmail\",\n  \"type\": \"object\",\n  \"description\": \"Email/password credentials for a user\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"is_disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether these credentials are disabled\"\n    },\n    \"logged_in_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of last login with these credentials\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when these credentials were created\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-credentials-email-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: CredentialsEmail
---
