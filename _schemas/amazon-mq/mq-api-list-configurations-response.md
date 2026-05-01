---
description: ListConfigurationsResponse schema from Amazon MQ API
layout: schema
name: ListConfigurationsResponse
properties_list:
- description: ''
  name: Configurations
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-list-configurations-response-schema.json
slug: mq-api-list-configurations-response
source_filename: mq-api-list-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-configurations-response-schema.json\",\n  \"title\": \"ListConfigurationsResponse\",\n  \"description\": \"ListConfigurationsResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Configurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurations\"\n          },\n          \"description\": \"The list of all revisions for the specified configuration.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\": \"The maximum number\
  \ of configurations that Amazon MQ can return per page (20 by default). This value must be an integer from 5 to 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token that specifies the next page of results Amazon MQ should return. To request the first page, leave nextToken empty.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-configurations-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListConfigurationsResponse
---
