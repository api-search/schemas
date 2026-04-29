---
description: StopCrawlerRequest schema from Amazon Glue API
layout: schema
name: StopCrawlerRequest
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-stop-crawler-request-schema.json
slug: glue-stop-crawler-request
source_filename: glue-stop-crawler-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-crawler-request-schema.json\",\n  \"title\": \"StopCrawlerRequest\",\n  \"description\": \"StopCrawlerRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the crawler to stop.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-crawler-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StopCrawlerRequest
---
