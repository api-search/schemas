---
description: The list of information about logs to be enabled for the specified broker.
layout: schema
name: PendingLogs
properties_list:
- description: ''
  name: Audit
  type: object
- description: ''
  name: General
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-pending-logs-schema.json
slug: mq-api-pending-logs
source_filename: mq-api-pending-logs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-pending-logs-schema.json\",\n  \"title\": \"PendingLogs\",\n  \"description\": \"The list of information about logs to be enabled for the specified broker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Audit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audit\"\n          },\n          \"description\": \"Enables audit logging. Every user management action made using JMX or the ActiveMQ Web Console is logged.\"\n        }\n      ]\n    },\n    \"General\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"general\"\n          },\n          \"description\": \"Enables general\
  \ logging.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-pending-logs-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PendingLogs
---
