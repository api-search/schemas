---
description: ''
layout: schema
name: RecordTypeInfos
properties_list:
- description: ''
  name: 012000000000000AAA
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record-type-infos-schema.json
slug: salesforce-record-type-infos
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"012000000000000AAA\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"available\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"defaultRecordTypeMapping\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"master\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"recordTypeId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"available\",\n        \"defaultRecordTypeMapping\",\n        \"master\",\n        \"name\",\n        \"recordTypeId\"\n      ]\n    }\n  },\n  \"required\": [\n    \"012000000000000AAA\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordTypeInfos\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record-type-infos-schema.json
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
title: RecordTypeInfos
---
