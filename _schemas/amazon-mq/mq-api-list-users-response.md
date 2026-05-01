---
description: ListUsersResponse schema from Amazon MQ API
layout: schema
name: ListUsersResponse
properties_list:
- description: ''
  name: BrokerId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Users
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-list-users-response-schema.json
slug: mq-api-list-users-response
source_filename: mq-api-list-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-users-response-schema.json\",\n  \"title\": \"ListUsersResponse\",\n  \"description\": \"ListUsersResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin5Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\": \"Required. The maximum number of ActiveMQ users that\
  \ can be returned per page (20 by default). This value must be an integer from 5 to 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token that specifies the next page of results Amazon MQ should return. To request the first page, leave nextToken empty.\"\n        }\n      ]\n    },\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUserSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"users\"\n          },\n          \"description\": \"Required. The list of all ActiveMQ usernames for the specified broker. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-users-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListUsersResponse
---
