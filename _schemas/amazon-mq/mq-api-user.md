---
description: A user associated with the broker. For RabbitMQ brokers, one and only one administrative user is accepted and created when a broker is first provisioned. All subsequent broker users are created by making RabbitMQ API calls directly to brokers or via the RabbitMQ web console.
layout: schema
name: User
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
- description: ''
  name: Username
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-user-schema.json
slug: mq-api-user
source_filename: mq-api-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A user associated with the broker. For RabbitMQ brokers, one and only one administrative user is accepted and created when a broker is first provisioned. All subsequent broker users are created by making RabbitMQ API calls directly to brokers or via the RabbitMQ web console.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConsoleAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"consoleAccess\"\n          },\n          \"description\": \"Enables access to the ActiveMQ Web Console for the ActiveMQ user. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    },\n    \"Groups\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groups\"\n          },\n          \"description\": \"The list of groups (20 maximum) to which the ActiveMQ user belongs. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"password\"\n          },\n          \"description\": \"Required. The password of the user. This value must be at least 12 characters long, must contain at least 4 unique characters, and must not contain commas, colons, or equal signs (,:=).\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"<p>important><title>Amazon MQ for ActiveMQ</title> <para>For ActiveMQ brokers, this value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.</p>/important> <important><title>Amazon MQ for RabbitMQ</title> <p>For RabbitMQ brokers, this value can contain only alphanumeric characters, dashes, periods, underscores (- . _). This value must not contain a tilde (~) character. Amazon MQ prohibts using guest as a valid usename. This value must be 2-100 characters long.</p></important></para>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Username\",\n    \"Password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-user-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: User
---
