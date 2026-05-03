---
description: Authentication request and response structures for the Login command, which returns a session token for subsequent API calls.
layout: schema
name: Reolink Login
properties_list:
- description: Login request payload
  name: request
  type: object
- description: Login response containing the session token
  name: response
  type: object
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/login.json
slug: login
source_filename: login.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"login.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Login\",\n  \"description\": \"Authentication request and response structures for the Login command, which returns a session token for subsequent API calls.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request\": {\n      \"type\": \"object\",\n      \"description\": \"Login request payload\",\n      \"properties\": {\n        \"cmd\": {\n          \"type\": \"string\",\n          \"const\": \"Login\"\n        },\n        \"action\": {\n          \"type\": \"integer\",\n          \"const\": 0\n        },\n        \"param\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"User\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"userName\": {\n                  \"type\": \"string\",\n                  \"description\": \"Account username\"\n                },\n               \
  \ \"password\": {\n                  \"type\": \"string\",\n                  \"description\": \"Account password\"\n                }\n              },\n              \"required\": [\"userName\", \"password\"]\n            }\n          },\n          \"required\": [\"User\"]\n        }\n      },\n      \"required\": [\"cmd\", \"action\", \"param\"]\n    },\n    \"response\": {\n      \"type\": \"object\",\n      \"description\": \"Login response containing the session token\",\n      \"properties\": {\n        \"cmd\": {\n          \"type\": \"string\",\n          \"const\": \"Login\"\n        },\n        \"code\": {\n          \"type\": \"integer\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Token\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"leaseTime\": {\n                  \"type\": \"integer\",\n                  \"description\": \"Token validity period in seconds\"\n\
  \                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Authentication token to use in subsequent requests\"\n                }\n              },\n              \"required\": [\"leaseTime\", \"name\"]\n            }\n          },\n          \"required\": [\"Token\"]\n        }\n      },\n      \"required\": [\"cmd\", \"code\", \"value\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/login.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Login
---
