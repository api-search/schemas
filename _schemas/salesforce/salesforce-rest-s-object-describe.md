---
description: Metadata describing a Salesforce SObject type, including its fields, relationships, and capabilities.
layout: schema
name: SObjectDescribe
properties_list:
- description: The API name of the SObject type.
  name: name
  type: string
- description: The user-facing singular label for this object type.
  name: label
  type: string
- description: The user-facing plural label for this object type.
  name: labelPlural
  type: string
- description: The three-character key prefix used in record IDs for this type.
  name: keyPrefix
  type: string
- description: Whether records of this type can be queried with SOQL.
  name: queryable
  type: boolean
- description: Whether records of this type can be searched with SOSL.
  name: searchable
  type: boolean
- description: Whether new records of this type can be created via the API.
  name: createable
  type: boolean
- description: Whether existing records of this type can be updated via the API.
  name: updateable
  type: boolean
- description: Whether records of this type can be deleted via the API.
  name: deletable
  type: boolean
- description: Detailed metadata for each field on this SObject type.
  name: fields
  type: array
- description: Map of REST endpoint URLs for this SObject type.
  name: urls
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-s-object-describe-schema.json
slug: salesforce-rest-s-object-describe
source_filename: salesforce-rest-s-object-describe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata describing a Salesforce SObject type, including its fields, relationships, and capabilities.\\n\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The API name of the SObject type.\",\n      \"example\": \"Example Title\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The user-facing singular label for this object type.\",\n      \"example\": \"Example Title\"\n    },\n    \"labelPlural\": {\n      \"type\": \"string\",\n      \"description\": \"The user-facing plural label for this object type.\",\n      \"example\": \"example_value\"\n    },\n    \"keyPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"The three-character key prefix used in record IDs for this type.\",\n      \"example\": \"example_value\"\n    },\n    \"queryable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether records of this type can\
  \ be queried with SOQL.\",\n      \"example\": true\n    },\n    \"searchable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether records of this type can be searched with SOSL.\",\n      \"example\": true\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether new records of this type can be created via the API.\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether existing records of this type can be updated via the API.\",\n      \"example\": true\n    },\n    \"deletable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether records of this type can be deleted via the API.\",\n      \"example\": true\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed metadata for each field on this SObject type.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n      \
  \    \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The API name of the field.\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"The user-facing label for this field.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The data type of the field (e.g., string, boolean, date, reference, picklist).\\n\"\n          },\n          \"nillable\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this field can be set to null.\"\n          },\n          \"updateable\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this field can be updated via the API.\"\n          },\n          \"createable\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this field can be set when creating a record.\"\n          },\n          \"length\": {\n            \"type\": \"integer\",\n\
  \            \"description\": \"Maximum character length for string fields. Zero for non-string fields.\\n\"\n          }\n        }\n      }\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"description\": \"Map of REST endpoint URLs for this SObject type.\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SObjectDescribe\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-s-object-describe-schema.json
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
title: SObjectDescribe
---
