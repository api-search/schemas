---
description: ListBrokersResponse schema from Amazon MQ API
layout: schema
name: ListBrokersResponse
properties_list:
- description: ''
  name: BrokerSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-list-brokers-response-schema.json
slug: mq-api-list-brokers-response
source_filename: mq-api-list-brokers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-brokers-response-schema.json\",\n  \"title\": \"ListBrokersResponse\",\n  \"description\": \"ListBrokersResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBrokerSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerSummaries\"\n          },\n          \"description\": \"A list of information about all brokers.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token that specifies the next page of results Amazon\
  \ MQ should return. To request the first page, leave nextToken empty.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-brokers-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListBrokersResponse
---
