---
description: Updates the information for an ActiveMQ user.
layout: schema
name: UpdateUserRequest
properties_list:
- description: ''
  name: ConsoleAccess
  type: object
- description: ''
  name: Groups
  type: object
- description: ''
  name: Password
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-update-user-request-schema.json
slug: mq-api-update-user-request
source_filename: mq-api-update-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-user-request-schema.json\",\n  \"title\": \"UpdateUserRequest\",\n  \"description\": \"Updates the information for an ActiveMQ user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConsoleAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"consoleAccess\"\n          },\n          \"description\": \"Enables access to the the ActiveMQ Web Console for the ActiveMQ user.\"\n        }\n      ]\n    },\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groups\"\n          },\n          \"description\": \"The list of groups (20 maximum) to which the\
  \ ActiveMQ user belongs. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"password\"\n          },\n          \"description\": \"The password of the user. This value must be at least 12 characters long, must contain at least 4 unique characters, and must not contain commas, colons, or equal signs (,:=).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-user-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateUserRequest
---
