---
description: ''
layout: schema
name: Registration-InitializeRequest
properties_list:
- description: ''
  name: userdata
  type: object
- description: ''
  name: customdata
  type: object
- description: ''
  name: password
  type: string
- description: ''
  name: recaptcha
  type: string
- description: ''
  name: verificationmethod
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-registration-initialize-request-schema.json
slug: salesforce-registration-initialize-request
source_filename: salesforce-registration-initialize-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"userdata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"firstName\",\n        \"lastName\",\n        \"email\",\n        \"username\"\n      ]\n    },\n    \"customdata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mobilePhone\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"streetAddress\": {\n          \"type\": \"string\",\n          \"example\"\
  : \"example_value\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"privacyPolicy\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"mobilePhone\",\n        \"streetAddress\",\n        \"city\",\n        \"state\",\n        \"zip\",\n        \"privacyPolicy\"\n      ]\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"recaptcha\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"verificationmethod\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"userdata\",\n    \"customdata\"\
  ,\n    \"password\",\n    \"recaptcha\",\n    \"verificationmethod\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Registration-InitializeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-registration-initialize-request-schema.json
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
title: Registration-InitializeRequest
---
