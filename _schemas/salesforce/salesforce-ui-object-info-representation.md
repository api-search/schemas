---
description: Metadata about a Salesforce object
layout: schema
name: ObjectInfoRepresentation
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: labelPlural
  type: string
- description: ''
  name: keyPrefix
  type: string
- description: ''
  name: createable
  type: boolean
- description: ''
  name: updateable
  type: boolean
- description: ''
  name: deleteable
  type: boolean
- description: ''
  name: queryable
  type: boolean
- description: Field metadata indexed by field API name
  name: fields
  type: object
- description: ''
  name: recordTypeInfos
  type: object
- description: ''
  name: themeInfo
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-object-info-representation-schema.json
slug: salesforce-ui-object-info-representation
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata about a Salesforce object\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"labelPlural\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"keyPrefix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deleteable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"queryable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Field metadata indexed by field API name\",\n      \"example\": \"example_value\"\
  \n    },\n    \"recordTypeInfos\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"themeInfo\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"color\": {\n          \"type\": \"string\"\n        },\n        \"iconUrl\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectInfoRepresentation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-object-info-representation-schema.json
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
title: ObjectInfoRepresentation
---
