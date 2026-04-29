---
description: DeleteBrokerResponse schema from Amazon MQ API
layout: schema
name: DeleteBrokerResponse
properties_list:
- description: ''
  name: BrokerId
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-delete-broker-response-schema.json
slug: mq-api-delete-broker-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-delete-broker-response-schema.json\",\n  \"title\": \"DeleteBrokerResponse\",\n  \"description\": \"DeleteBrokerResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-delete-broker-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeleteBrokerResponse
---
