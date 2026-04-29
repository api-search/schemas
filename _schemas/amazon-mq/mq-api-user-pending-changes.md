---
description: Returns information about the status of the changes pending for the ActiveMQ user.
layout: schema
name: UserPendingChanges
properties_list:
- description: ''
  name: ConsoleAccess
  type: object
- description: ''
  name: Groups
  type: object
- description: ''
  name: PendingChange
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-user-pending-changes-schema.json
slug: mq-api-user-pending-changes
source_filename: mq-api-user-pending-changes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-user-pending-changes-schema.json\",\n  \"title\": \"UserPendingChanges\",\n  \"description\": \"Returns information about the status of the changes pending for the ActiveMQ user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConsoleAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"consoleAccess\"\n          },\n          \"description\": \"Enables access to the the ActiveMQ Web Console for the ActiveMQ user.\"\n        }\n      ]\n    },\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groups\"\n          },\n          \"description\": \"The list\
  \ of groups (20 maximum) to which the ActiveMQ user belongs. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.\"\n        }\n      ]\n    },\n    \"PendingChange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingChange\"\n          },\n          \"description\": \"Required. The type of change pending for the ActiveMQ user.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PendingChange\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-user-pending-changes-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UserPendingChanges
---
