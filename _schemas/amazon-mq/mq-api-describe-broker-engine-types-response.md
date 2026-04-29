---
description: DescribeBrokerEngineTypesResponse schema from Amazon MQ API
layout: schema
name: DescribeBrokerEngineTypesResponse
properties_list:
- description: ''
  name: BrokerEngineTypes
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-describe-broker-engine-types-response-schema.json
slug: mq-api-describe-broker-engine-types-response
source_filename: mq-api-describe-broker-engine-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-broker-engine-types-response-schema.json\",\n  \"title\": \"DescribeBrokerEngineTypesResponse\",\n  \"description\": \"DescribeBrokerEngineTypesResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerEngineTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBrokerEngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerEngineTypes\"\n          },\n          \"description\": \"List of available engine types and versions.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin5Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\"\
  : \"Required. The maximum number of engine types that can be returned per page (20 by default). This value must be an integer from 5 to 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token that specifies the next page of results Amazon MQ should return. To request the first page, leave nextToken empty.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-broker-engine-types-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeBrokerEngineTypesResponse
---
