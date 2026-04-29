---
description: ''
layout: schema
name: SuccessfulUserInfo
properties_list:
- description: ''
  name: sub
  type: string
- description: ''
  name: user_id
  type: string
- description: ''
  name: organization_id
  type: string
- description: ''
  name: preferred_username
  type: string
- description: ''
  name: nickname
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: email_verified
  type: boolean
- description: ''
  name: given_name
  type: string
- description: ''
  name: family_name
  type: string
- description: ''
  name: zoneinfo
  type: string
- description: ''
  name: photos
  type: object
- description: ''
  name: profile
  type: string
- description: ''
  name: picture
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: is_salesforce_integration_user
  type: boolean
- description: ''
  name: urls
  type: object
- description: ''
  name: active
  type: boolean
- description: ''
  name: user_type
  type: string
- description: ''
  name: language
  type: string
- description: ''
  name: locale
  type: string
- description: ''
  name: utcOffset
  type: integer
- description: ''
  name: updated_at
  type: string
- description: ''
  name: is_app_installed
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-user-info-schema.json
slug: salesforce-successful-user-info
source_filename: salesforce-successful-user-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"sub\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"organization_id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"preferred_username\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"email_verified\": {\n      \"type\": \"boolean\",\n      \"example\": \"user@example.com\"\n    },\n    \"given_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"family_name\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"zoneinfo\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"photos\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"picture\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"thumbnail\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"picture\",\n        \"thumbnail\"\n      ]\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"country\": {\n          \"type\": \"string\",\n          \"example\": 42\n        }\n      },\n      \"required\": [\n        \"country\"\n      ]\n    },\n    \"is_salesforce_integration_user\": {\n      \"type\"\
  : \"boolean\",\n      \"example\": true\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enterprise\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"metadata\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"partner\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"rest\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"sobjects\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"search\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"query\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"recent\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n     \
  \   },\n        \"tooling_soap\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"tooling_rest\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"profile\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"feeds\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"groups\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"users\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"feed_items\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"feed_elements\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"custom_domain\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\
  \n        }\n      },\n      \"required\": [\n        \"enterprise\",\n        \"metadata\",\n        \"partner\",\n        \"rest\",\n        \"sobjects\",\n        \"search\",\n        \"query\",\n        \"recent\",\n        \"tooling_soap\",\n        \"tooling_rest\",\n        \"profile\",\n        \"feeds\",\n        \"groups\",\n        \"users\",\n        \"feed_items\",\n        \"feed_elements\",\n        \"custom_domain\"\n      ]\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"user_type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"utcOffset\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\
  \n    },\n    \"is_app_installed\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"sub\",\n    \"user_id\",\n    \"organization_id\",\n    \"preferred_username\",\n    \"nickname\",\n    \"name\",\n    \"email\",\n    \"email_verified\",\n    \"given_name\",\n    \"family_name\",\n    \"zoneinfo\",\n    \"photos\",\n    \"profile\",\n    \"picture\",\n    \"address\",\n    \"is_salesforce_integration_user\",\n    \"urls\",\n    \"active\",\n    \"user_type\",\n    \"language\",\n    \"locale\",\n    \"utcOffset\",\n    \"updated_at\",\n    \"is_app_installed\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulUserInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-user-info-schema.json
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
title: SuccessfulUserInfo
---
