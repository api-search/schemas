---
description: BatchGetCrawlersRequest schema from Amazon Glue API
layout: schema
name: BatchGetCrawlersRequest
properties_list:
- description: ''
  name: CrawlerNames
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-crawlers-request-schema.json
slug: glue-batch-get-crawlers-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-crawlers-request-schema.json\",\n  \"title\": \"BatchGetCrawlersRequest\",\n  \"description\": \"BatchGetCrawlersRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrawlerNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerNameList\"\n        },\n        {\n          \"description\": \"A list of crawler names, which might be the names returned from the <code>ListCrawlers</code> operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CrawlerNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-crawlers-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetCrawlersRequest
---
