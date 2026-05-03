---
description: The response structure returned by the Salesforce REST API for SOQL query operations
layout: schema
name: Salesforce SOQL Query Result
properties_list:
- description: Total number of records matching the query
  name: totalSize
  type: integer
- description: Whether all results have been returned. False if there are more pages.
  name: done
  type: boolean
- description: URL to retrieve the next batch of records when done is false
  name: nextRecordsUrl
  type: string
- description: Array of sObject records returned by the query
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforcecom
schema_file: json-schema/salesforcecom-query-result-schema.json
slug: salesforcecom-query-result
source_filename: salesforcecom-query-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salesforcecom/json-schema/salesforcecom-query-result-schema.json\",\n  \"title\": \"Salesforce SOQL Query Result\",\n  \"description\": \"The response structure returned by the Salesforce REST API for SOQL query operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records matching the query\"\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether all results have been returned. False if there are more pages.\"\n    },\n    \"nextRecordsUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to retrieve the next batch of records when done is false\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"Array of sObject records returned by the query\",\n      \"items\": {\n        \"$ref\":\
  \ \"#/$defs/sObject\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"sObject\": {\n      \"type\": \"object\",\n      \"description\": \"A Salesforce record\",\n      \"properties\": {\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\"\n            },\n            \"url\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"totalSize\", \"done\", \"records\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforcecom/refs/heads/main/json-schema/salesforcecom-query-result-schema.json
tags:
- CRM
- Cloud
- Sales
- Marketing
- Automation
- AI
title: Salesforce SOQL Query Result
---
