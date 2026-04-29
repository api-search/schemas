---
description: ListConfigurationRevisionsResponse schema from Amazon MQ API
layout: schema
name: ListConfigurationRevisionsResponse
properties_list:
- description: ''
  name: ConfigurationId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Revisions
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-list-configuration-revisions-response-schema.json
slug: mq-api-list-configuration-revisions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-configuration-revisions-response-schema.json\",\n  \"title\": \"ListConfigurationRevisionsResponse\",\n  \"description\": \"ListConfigurationRevisionsResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurationId\"\n          },\n          \"description\": \"The unique ID that Amazon MQ generates for the configuration.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\":\
  \ \"The maximum number of configuration revisions that can be returned per page (20 by default). This value must be an integer from 5 to 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token that specifies the next page of results Amazon MQ should return. To request the first page, leave nextToken empty.\"\n        }\n      ]\n    },\n    \"Revisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfConfigurationRevision\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revisions\"\n          },\n          \"description\": \"The list of all revisions for the specified configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-configuration-revisions-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListConfigurationRevisionsResponse
---
