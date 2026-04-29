---
description: ''
layout: schema
name: Record2
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: website
  type: string
- description: ''
  name: numberOfEmployees
  type: string
- description: ''
  name: industry
  type: string
- description: ''
  name: Contacts
  type: object
- description: ''
  name: childAccounts
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record2-schema.json
slug: salesforce-record2
source_filename: salesforce-record2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"referenceId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"referenceId\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"numberOfEmployees\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Contacts\": {\n      \"type\": \"object\",\n      \"properties\":\
  \ {\n        \"records\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"attributes\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"referenceId\": {\n                    \"type\": \"string\",\n                    \"example\": \"500123\"\n                  }\n                },\n                \"required\": [\n                  \"type\",\n                  \"referenceId\"\n                ]\n              },\n              \"lastname\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"Title\": {\n                \"type\": \"string\",\n                \"example\"\
  : \"Example Title\"\n              },\n              \"email\": {\n                \"type\": \"string\",\n                \"example\": \"user@example.com\"\n              }\n            },\n            \"required\": [\n              \"attributes\",\n              \"lastname\",\n              \"email\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"records\"\n      ]\n    },\n    \"childAccounts\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"records\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"attributes\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"referenceId\": {\n    \
  \                \"type\": \"string\",\n                    \"example\": \"500123\"\n                  }\n                },\n                \"required\": [\n                  \"type\",\n                  \"referenceId\"\n                ]\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"phone\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"website\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"numberOfEmployees\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"industry\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"\
  attributes\",\n              \"name\",\n              \"phone\",\n              \"website\",\n              \"numberOfEmployees\",\n              \"industry\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"records\"\n      ]\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"name\",\n    \"phone\",\n    \"website\",\n    \"numberOfEmployees\",\n    \"industry\",\n    \"Contacts\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record2-schema.json
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
title: Record2
---
