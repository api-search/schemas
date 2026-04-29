---
description: Returns a list of all broker users. Does not apply to RabbitMQ brokers.
layout: schema
name: UserSummary
properties_list:
- description: ''
  name: PendingChange
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-user-summary-schema.json
slug: mq-api-user-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-user-summary-schema.json\",\n  \"title\": \"UserSummary\",\n  \"description\": \"Returns a list of all broker users. Does not apply to RabbitMQ brokers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PendingChange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingChange\"\n          },\n          \"description\": \"The type of change pending for the broker user.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"Required. The username of the broker user. This value can\
  \ contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-user-summary-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UserSummary
---
