---
description: <p>A list of information about the configuration.</p> <important><p>Does not apply to RabbitMQ brokers.</p></important>
layout: schema
name: ConfigurationId
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Revision
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-configuration-id-schema.json
slug: mq-api-configuration-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configuration-id-schema.json\",\n  \"title\": \"ConfigurationId\",\n  \"description\": \"<p>A list of information about the configuration.</p> <important><p>Does not apply to RabbitMQ brokers.</p></important>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the configuration.\"\n        }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revision\"\n          },\n          \"description\": \"\
  The revision number of the configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configuration-id-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigurationId
---
