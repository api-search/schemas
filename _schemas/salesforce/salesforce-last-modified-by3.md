---
description: ''
layout: schema
name: LastModifiedBy3
properties_list:
- description: ''
  name: displayValue
  type: string
- description: ''
  name: value
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-last-modified-by3-schema.json
slug: salesforce-last-modified-by3
source_filename: salesforce-last-modified-by3-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayValue\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"childRelationships\": {\n          \"type\": \"object\",\n          \"example\": \"example_value\"\n        },\n        \"eTag\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"fields\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Id\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"displayValue\": {\n                  \"type\": \"['string', 'null']\",\n                  \"example\": \"example_value\"\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                \
  \  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"displayValue\",\n                \"value\"\n              ]\n            },\n            \"Name\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"displayValue\": {\n                  \"type\": \"['string', 'null']\",\n                  \"example\": \"example_value\"\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"displayValue\",\n                \"value\"\n              ]\n            }\n          },\n          \"required\": [\n            \"Id\",\n            \"Name\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"lastModifiedById\": {\n          \"type\": \"\
  string\",\n          \"example\": \"500123\"\n        },\n        \"lastModifiedDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"recordTypeId\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"500123\"\n        },\n        \"recordTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"systemModstamp\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"weakEtag\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"childRelationships\",\n        \"eTag\",\n        \"fields\",\n        \"id\",\n        \"lastModifiedById\",\n        \"lastModifiedDate\",\n        \"recordTypeId\",\n        \"recordTypeInfo\",\n        \"systemModstamp\",\n        \"weakEtag\"\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"displayValue\",\n    \"value\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LastModifiedBy3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-last-modified-by3-schema.json
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
title: LastModifiedBy3
---
