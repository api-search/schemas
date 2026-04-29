---
description: ''
layout: schema
name: ProjectAccessRequest
properties_list:
- description: Array of person IDs to grant access
  name: grant
  type: array
- description: Array of person IDs to revoke access
  name: revoke
  type: array
- description: New people to invite to the project
  name: create
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectaccessrequest-schema.json
slug: projectaccessrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/projectaccessrequest-schema.json\",\n  \"title\": \"ProjectAccessRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grant\": {\n      \"type\": \"array\",\n      \"description\": \"Array of person IDs to grant access\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"revoke\": {\n      \"type\": \"array\",\n      \"description\": \"Array of person IDs to revoke access\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"create\": {\n      \"type\": \"array\",\n      \"description\": \"New people to invite to the project\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"name\",\n          \"email_address\"\n        ],\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Full\
  \ name of the new person\"\n          },\n          \"email_address\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"Email address of the new person\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"Job title\"\n          },\n          \"company_name\": {\n            \"type\": \"string\",\n            \"description\": \"Company name\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/projectaccessrequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectAccessRequest
---
