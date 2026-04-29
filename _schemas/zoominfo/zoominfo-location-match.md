---
description: ''
layout: schema
name: LocationMatch
properties_list:
- description: ''
  name: companyId
  type: integer
- description: ''
  name: address
  type: object
- description: ''
  name: addressStatus
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-location-match-schema.json
slug: zoominfo-location-match
source_filename: zoominfo-location-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"example\": \"San Francisco\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"example\": \"CA\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"zipCode\": {\n          \"type\": \"string\",\n          \"example\": \"94105\"\n        }\n      },\n      \"required\": [\n        \"street\",\n        \"city\",\n        \"state\",\n        \"country\",\n        \"zipCode\"\n      ]\n    },\n    \"addressStatus\": {\n      \"type\": \"string\",\n      \"example\": \"123 Main Street\"\n    }\n  },\n\
  \  \"required\": [\n    \"companyId\",\n    \"address\",\n    \"addressStatus\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LocationMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-location-match-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: LocationMatch
---
