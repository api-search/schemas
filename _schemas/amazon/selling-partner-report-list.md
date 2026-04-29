---
description: ReportList schema from Amazon Selling Partner API
layout: schema
name: ReportList
properties_list:
- description: ''
  name: reports
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-report-list-schema.json
slug: selling-partner-report-list
source_filename: selling-partner-report-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"reports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Report\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-report-list-schema.json\",\n  \"description\": \"ReportList schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-report-list-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ReportList
---
