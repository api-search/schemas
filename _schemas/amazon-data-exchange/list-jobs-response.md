---
description: Response containing a list of jobs.
layout: schema
name: List Jobs Response
properties_list:
- description: ''
  name: Jobs
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/list-jobs-response-schema.json
slug: list-jobs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/list-jobs-response-schema.json\",\n  \"title\": \"List Jobs Response\",\n  \"description\": \"Response containing a list of jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"job-schema.json\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/list-jobs-response-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: List Jobs Response
---
