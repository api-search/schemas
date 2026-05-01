---
description: GetCrawlersResponse schema from Amazon Glue API
layout: schema
name: GetCrawlersResponse
properties_list:
- description: ''
  name: Crawlers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-crawlers-response-schema.json
slug: glue-get-crawlers-response
source_filename: glue-get-crawlers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-crawlers-response-schema.json\",\n  \"title\": \"GetCrawlersResponse\",\n  \"description\": \"GetCrawlersResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Crawlers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerList\"\n        },\n        {\n          \"description\": \"A list of crawler metadata.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list has not reached the end of those defined in this customer account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-crawlers-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetCrawlersResponse
---
