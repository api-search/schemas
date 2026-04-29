---
description: ''
layout: schema
name: CreatemanagedeventsubscriptionRequest
properties_list:
- description: ''
  name: FullName
  type: string
- description: ''
  name: Metadata
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-createmanagedeventsubscription-request-schema.json
slug: salesforce-createmanagedeventsubscription-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"topicName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"defaultReplay\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"errorRecoveryReplay\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"label\",\n        \"topicName\",\n        \"defaultReplay\",\n        \"state\",\n        \"errorRecoveryReplay\"\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"FullName\",\n    \"Metadata\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreatemanagedeventsubscriptionRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-createmanagedeventsubscription-request-schema.json
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
title: CreatemanagedeventsubscriptionRequest
---
