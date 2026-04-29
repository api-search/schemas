---
description: SOAP envelope containing a query definition with schema, operation, selected fields, conditions, and pagination parameters.
layout: schema
name: QueryDefinition
properties_list:
- description: ''
  name: queryDef
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-query-definition-schema.json
slug: adobe-campaign-classic-query-definition
source_filename: adobe-campaign-classic-query-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-query-definition-schema.json\",\n  \"title\": \"QueryDefinition\",\n  \"description\": \"SOAP envelope containing a query definition with schema, operation, selected fields, conditions, and pagination parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryDef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"schema\": {\n          \"type\": \"string\",\n          \"description\": \"Target schema name (e.g., nms:recipient, nms:delivery).\"\n        },\n        \"operation\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"get\",\n            \"getIfExists\",\n            \"select\",\n            \"count\"\n          ],\n          \"description\": \"Query operation type. get returns single record (error if missing), getIfExists\
  \ returns single or null, select returns multiple records, count returns record count.\"\n        },\n        \"lineCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of records to return.\"\n        },\n        \"startLine\": {\n          \"type\": \"integer\",\n          \"description\": \"Starting offset for pagination.\"\n        },\n        \"select\": {\n          \"type\": \"object\",\n          \"description\": \"Field selection using XPath node elements.\"\n        },\n        \"where\": {\n          \"type\": \"object\",\n          \"description\": \"WHERE conditions using condition elements with expr attributes.\"\n        },\n        \"orderBy\": {\n          \"type\": \"object\",\n          \"description\": \"ORDER BY clause with sortNode elements.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-query-definition-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: QueryDefinition
---
