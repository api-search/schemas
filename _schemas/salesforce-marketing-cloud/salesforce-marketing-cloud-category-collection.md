---
description: Paginated collection of asset categories
layout: schema
name: CategoryCollection
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: page
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: items
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-category-collection-schema.json
slug: salesforce-marketing-cloud-category-collection
source_filename: salesforce-marketing-cloud-category-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CategoryCollection\",\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of asset categories\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"items\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-category-collection-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: CategoryCollection
---
