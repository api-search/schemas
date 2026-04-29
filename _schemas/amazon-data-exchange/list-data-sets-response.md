---
description: Response containing a list of data sets.
layout: schema
name: List Data Sets Response
properties_list:
- description: ''
  name: DataSets
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/list-data-sets-response-schema.json
slug: list-data-sets-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/list-data-sets-response-schema.json\",\n  \"title\": \"List Data Sets Response\",\n  \"description\": \"Response containing a list of data sets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataSets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"data-set-schema.json\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/list-data-sets-response-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: List Data Sets Response
---
