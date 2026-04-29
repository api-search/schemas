---
description: Response containing a list of event actions.
layout: schema
name: List Event Actions Response
properties_list:
- description: ''
  name: EventActions
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/list-event-actions-response-schema.json
slug: list-event-actions-response
source_filename: list-event-actions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/list-event-actions-response-schema.json\",\n  \"title\": \"List Event Actions Response\",\n  \"description\": \"Response containing a list of event actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventActions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"event-action-schema.json\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/list-event-actions-response-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: List Event Actions Response
---
