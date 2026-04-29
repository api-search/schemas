---
description: Metadata for a single field
layout: schema
name: FieldRepresentation
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: dataType
  type: string
- description: ''
  name: required
  type: boolean
- description: ''
  name: updateable
  type: boolean
- description: ''
  name: createable
  type: boolean
- description: ''
  name: nillable
  type: boolean
- description: ''
  name: referenceToInfos
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-field-representation-schema.json
slug: salesforce-ui-field-representation
source_filename: salesforce-ui-field-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata for a single field\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"example\": \"Address\",\n      \"enum\": [\n        \"Address\",\n        \"Boolean\",\n        \"Currency\",\n        \"Date\",\n        \"DateTime\",\n        \"Double\",\n        \"Email\",\n        \"Id\",\n        \"Integer\",\n        \"Long\",\n        \"MultiPicklist\",\n        \"Percent\",\n        \"Phone\",\n        \"Picklist\",\n        \"Reference\",\n        \"String\",\n        \"TextArea\",\n        \"Time\",\n        \"Url\"\n      ]\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n   \
  \ \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"nillable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"referenceToInfos\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"apiName\": {\n            \"type\": \"string\"\n          },\n          \"nameFields\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldRepresentation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-field-representation-schema.json
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
title: FieldRepresentation
---
