---
description: OrganizationAcl from LinkedIn API
layout: schema
name: OrganizationAcl
properties_list:
- description: ''
  name: organization
  type: string
- description: ''
  name: roleAssignee
  type: string
- description: ''
  name: role
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: created
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-organization-acl-schema.json
slug: linkedin-regulations-data-portability-organization-acl
source_filename: linkedin-regulations-data-portability-organization-acl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-organization-acl-schema.json\",\n  \"title\": \"OrganizationAcl\",\n  \"description\": \"OrganizationAcl from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organization\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:organization:10002687\"\n    },\n    \"roleAssignee\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:person:ABC123\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADMINISTRATOR\",\n        \"CONTENT_ADMIN\",\n        \"ANALYST\",\n        \"RECRUITING_POSTER\"\n      ],\n      \"example\": \"ADMINISTRATOR\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"APPROVED\",\n        \"PENDING\"\n      ],\n      \"example\": \"APPROVED\"\n   \
  \ },\n    \"created\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-organization-acl-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: OrganizationAcl
---
