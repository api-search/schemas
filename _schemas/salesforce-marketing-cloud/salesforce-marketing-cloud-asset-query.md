---
description: Advanced query object for searching assets
layout: schema
name: AssetQuery
properties_list:
- description: ''
  name: page
  type: object
- description: Query filter criteria
  name: query
  type: object
- description: ''
  name: sort
  type: array
- description: Specific fields to include in the response
  name: fields
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-asset-query-schema.json
slug: salesforce-marketing-cloud-asset-query
source_filename: salesforce-marketing-cloud-asset-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetQuery\",\n  \"type\": \"object\",\n  \"description\": \"Advanced query object for searching assets\",\n  \"properties\": {\n    \"page\": {\n      \"type\": \"object\"\n    },\n    \"query\": {\n      \"type\": \"object\",\n      \"description\": \"Query filter criteria\"\n    },\n    \"sort\": {\n      \"type\": \"array\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"Specific fields to include in the response\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-asset-query-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: AssetQuery
---
