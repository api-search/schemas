---
description: Response containing a list of assets.
layout: schema
name: List Revision Assets Response
properties_list:
- description: ''
  name: Assets
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/list-revision-assets-response-schema.json
slug: list-revision-assets-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/list-revision-assets-response-schema.json\",\n  \"title\": \"List Revision Assets Response\",\n  \"description\": \"Response containing a list of assets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Assets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"asset-schema.json\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/list-revision-assets-response-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: List Revision Assets Response
---
