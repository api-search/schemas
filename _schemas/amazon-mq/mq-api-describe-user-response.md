---
description: DescribeUserResponse schema from Amazon MQ API
layout: schema
name: DescribeUserResponse
properties_list:
- description: ''
  name: BrokerId
  type: object
- description: ''
  name: ConsoleAccess
  type: object
- description: ''
  name: Groups
  type: object
- description: ''
  name: Pending
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-describe-user-response-schema.json
slug: mq-api-describe-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-user-response-schema.json\",\n  \"title\": \"DescribeUserResponse\",\n  \"description\": \"DescribeUserResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n    },\n    \"ConsoleAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"consoleAccess\"\n          },\n          \"description\": \"Enables access to the the ActiveMQ Web Console\
  \ for the ActiveMQ user.\"\n        }\n      ]\n    },\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groups\"\n          },\n          \"description\": \"The list of groups (20 maximum) to which the ActiveMQ user belongs. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.\"\n        }\n      ]\n    },\n    \"Pending\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPendingChanges\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pending\"\n          },\n          \"description\": \"The status of the changes pending for the ActiveMQ user.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n     \
  \     \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"Required. The username of the ActiveMQ user. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-user-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeUserResponse
---
