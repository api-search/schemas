---
description: Provider schema from Availity API
layout: schema
name: Provider
properties_list:
- description: National Provider Identifier (NPI)
  name: npi
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: organizationName
  type: string
- description: ''
  name: taxId
  type: string
- description: ''
  name: serviceProviderNumber
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-provider-schema.json
slug: eligibility-provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-provider-schema.json\",\n  \"title\": \"Provider\",\n  \"description\": \"Provider schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"npi\"\n  ],\n  \"properties\": {\n    \"npi\": {\n      \"type\": \"string\",\n      \"description\": \"National Provider Identifier (NPI)\",\n      \"pattern\": \"^\\\\d{10}$\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"type\": \"string\"\n    },\n    \"serviceProviderNumber\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-provider-schema.json
tags: []
title: Provider
---
