---
description: ''
layout: schema
name: Actions
properties_list:
- description: ''
  name: Global
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-actions-schema.json
slug: salesforce-actions
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Global\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"actions\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"actionListContext\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"actionTarget\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"actionTargetType\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"apiName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"externalId\": {\n                \"type\": \"string\"\
  ,\n                \"example\": \"500123\"\n              },\n              \"iconUrl\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"isMassAction\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"label\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"lwcComponent\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"primaryColor\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"relatedListRecordId\": {\n                \"type\": \"['string', 'null']\",\n           \
  \     \"example\": \"500123\"\n              },\n              \"relatedSourceObject\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"section\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"sourceObject\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"subtype\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"targetObject\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"targetUrl\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"https://www.example.com\"\n              },\n              \"type\": {\n                \"type\": \"string\"\
  ,\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"actionListContext\",\n              \"actionTarget\",\n              \"actionTargetType\",\n              \"apiName\",\n              \"externalId\",\n              \"iconUrl\",\n              \"id\",\n              \"isMassAction\",\n              \"label\",\n              \"lwcComponent\",\n              \"primaryColor\",\n              \"relatedListRecordId\",\n              \"relatedSourceObject\",\n              \"section\",\n              \"sourceObject\",\n              \"subtype\",\n              \"targetObject\",\n              \"targetUrl\",\n              \"type\"\n            ]\n          }\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"url\": {\n          \"type\": \"string\"\
  ,\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"actions\",\n        \"links\",\n        \"url\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Global\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Actions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-actions-schema.json
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
title: Actions
---
