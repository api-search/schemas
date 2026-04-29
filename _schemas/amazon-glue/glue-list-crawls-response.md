---
description: ListCrawlsResponse schema from Amazon Glue API
layout: schema
name: ListCrawlsResponse
properties_list:
- description: ''
  name: Crawls
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-crawls-response-schema.json
slug: glue-list-crawls-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-crawls-response-schema.json\",\n  \"title\": \"ListCrawlsResponse\",\n  \"description\": \"ListCrawlsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Crawls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerHistoryList\"\n        },\n        {\n          \"description\": \"A list of <code>CrawlerHistory</code> objects representing the crawl runs that meet your criteria.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token for paginating the returned list of tokens, returned if the current segment of the list is not the last.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-crawls-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListCrawlsResponse
---
