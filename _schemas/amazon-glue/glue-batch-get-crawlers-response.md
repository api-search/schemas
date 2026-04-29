---
description: BatchGetCrawlersResponse schema from Amazon Glue API
layout: schema
name: BatchGetCrawlersResponse
properties_list:
- description: ''
  name: Crawlers
  type: object
- description: ''
  name: CrawlersNotFound
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-crawlers-response-schema.json
slug: glue-batch-get-crawlers-response
source_filename: glue-batch-get-crawlers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-crawlers-response-schema.json\",\n  \"title\": \"BatchGetCrawlersResponse\",\n  \"description\": \"BatchGetCrawlersResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Crawlers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerList\"\n        },\n        {\n          \"description\": \"A list of crawler definitions.\"\n        }\n      ]\n    },\n    \"CrawlersNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerNameList\"\n        },\n        {\n          \"description\": \"A list of names of crawlers that were not found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-crawlers-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetCrawlersResponse
---
