---
description: IdentityNamespaceInput schema
layout: schema
name: IdentityNamespaceInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: idType
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-identity-namespace-input-schema.json
slug: experience-platform-api-identity-namespace-input
source_filename: experience-platform-api-identity-namespace-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-identity-namespace-input-schema.json\",\n  \"title\": \"IdentityNamespaceInput\",\n  \"description\": \"IdentityNamespaceInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"code\",\n    \"idType\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"idType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"COOKIE\",\n        \"DEVICE\",\n        \"CROSS_DEVICE\",\n        \"EMAIL\",\n        \"PHONE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-identity-namespace-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: IdentityNamespaceInput
---
