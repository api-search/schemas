---
description: Schema for Salesforce Knowledge data categories used to organize and filter articles.
layout: schema
name: Salesforce Knowledge Data Category
properties_list:
- description: Display label for the data category
  name: label
  type: string
- description: API name for the data category
  name: name
  type: string
- description: URL of the data category resource
  name: url
  type: string
- description: Sub-categories under this category
  name: childCategories
  type: array
provider_name: Salesforce Knowledge Management
provider_slug: salesforce-knowledge-management
schema_file: json-schema/salesforce-knowledge-management-category-schema.json
slug: salesforce-knowledge-management-category
source_filename: salesforce-knowledge-management-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-knowledge-management/blob/main/json-schema/salesforce-knowledge-management-category-schema.json\",\n  \"title\": \"Salesforce Knowledge Data Category\",\n  \"description\": \"Schema for Salesforce Knowledge data categories used to organize and filter articles.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the data category\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"API name for the data category\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the data category resource\"\n    },\n    \"childCategories\": {\n      \"type\": \"array\",\n      \"description\": \"Sub-categories under this category\",\n      \"items\": {\n        \"$ref\": \"#\"\n      }\n\
  \    }\n  },\n  \"required\": [\"name\", \"label\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/json-schema/salesforce-knowledge-management-category-schema.json
tags:
- Articles
- CRM
- Customer Service
- Documentation
- Knowledge Management
- Support
title: Salesforce Knowledge Data Category
---
