---
description: ''
layout: schema
name: listMetadataResponse
properties_list:
- description: ''
  name: result
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-list-metadata-response-schema.json
slug: salesforce-list-metadata-response
source_filename: salesforce-list-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"createdById\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"createdByName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"createdDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fileName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fullName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"lastModifiedById\": {\n            \"\
  type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"lastModifiedByName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"lastModifiedDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"namespacePrefix\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"createdById\",\n          \"createdByName\",\n          \"createdDate\",\n          \"fileName\",\n          \"fullName\",\n          \"id\",\n          \"lastModifiedById\",\n          \"lastModifiedByName\",\n          \"lastModifiedDate\",\n          \"namespacePrefix\",\n          \"type\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"result\"\n  ],\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"listMetadataResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-list-metadata-response-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: listMetadataResponse
---
