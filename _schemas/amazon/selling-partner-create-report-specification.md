---
description: CreateReportSpecification schema from Amazon Selling Partner API
layout: schema
name: CreateReportSpecification
properties_list:
- description: ''
  name: reportType
  type: string
- description: ''
  name: dataStartTime
  type: string
- description: ''
  name: dataEndTime
  type: string
- description: ''
  name: marketplaceIds
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-create-report-specification-schema.json
slug: selling-partner-create-report-specification
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"reportType\",\n    \"marketplaceIds\"\n  ],\n  \"properties\": {\n    \"reportType\": {\n      \"type\": \"string\"\n    },\n    \"dataStartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"dataEndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"marketplaceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateReportSpecification\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-create-report-specification-schema.json\",\n  \"description\": \"CreateReportSpecification schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-create-report-specification-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CreateReportSpecification
---
