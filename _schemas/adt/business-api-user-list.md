---
description: List of site users.
layout: schema
name: UserList
properties_list:
- description: Array of users.
  name: users
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/business-api-user-list-schema.json
slug: business-api-user-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-user-list-schema.json\",\n  \"title\": \"UserList\",\n  \"description\": \"List of site users.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"users\": {\n      \"type\": \"array\",\n      \"description\": \"Array of users.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A user with access to a business site.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique user ID.\",\n            \"example\": \"usr-001\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Full name of the user.\",\n            \"example\": \"Jane Smith\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n  \
  \          \"description\": \"Email address.\",\n            \"example\": \"jsmith@example.com\"\n          },\n          \"role\": {\n            \"type\": \"string\",\n            \"description\": \"User role.\",\n            \"enum\": [\n              \"admin\",\n              \"manager\",\n              \"employee\",\n              \"contractor\"\n            ],\n            \"example\": \"employee\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-user-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: UserList
---
