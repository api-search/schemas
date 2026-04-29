---
description: ''
layout: schema
name: Organization
properties_list:
- description: Resource name of the organization.
  name: name
  type: string
- description: The display name of the organization.
  name: displayName
  type: string
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
schema_file: json-schema/openapi-organization-schema.json
slug: openapi-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the organization.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/json-schema/openapi-organization-schema.json
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
title: Organization
---
