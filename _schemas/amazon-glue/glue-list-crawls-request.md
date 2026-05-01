---
description: ListCrawlsRequest schema from Amazon Glue API
layout: schema
name: ListCrawlsRequest
properties_list:
- description: ''
  name: CrawlerName
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-crawls-request-schema.json
slug: glue-list-crawls-request
source_filename: glue-list-crawls-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-crawls-request-schema.json\",\n  \"title\": \"ListCrawlsRequest\",\n  \"description\": \"ListCrawlsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrawlerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the crawler whose runs you want to retrieve.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. The default is 20, and maximum is 100.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlsFilterList\"\
  \n        },\n        {\n          \"description\": \"Filters the crawls by the criteria you specify in a list of <code>CrawlsFilter</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CrawlerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-crawls-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListCrawlsRequest
---
