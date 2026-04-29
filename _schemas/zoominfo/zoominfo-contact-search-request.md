---
description: ''
layout: schema
name: ContactSearchRequest
properties_list:
- description: ''
  name: managementLevel
  type: string
- description: ''
  name: companyType
  type: string
- description: ''
  name: zipCode
  type: string
- description: ''
  name: locationSearchType
  type: string
- description: ''
  name: zipCodeRadiusMiles
  type: string
- description: ''
  name: techAttributeTagList
  type: string
- description: ''
  name: requiredFields
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-contact-search-request-schema.json
slug: zoominfo-contact-search-request
source_filename: zoominfo-contact-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"managementLevel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"companyType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"locationSearchType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"zipCodeRadiusMiles\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"techAttributeTagList\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"requiredFields\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"managementLevel\",\n    \"companyType\",\n    \"zipCode\",\n    \"locationSearchType\",\n    \"zipCodeRadiusMiles\",\n    \"techAttributeTagList\",\n    \"requiredFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ContactSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-contact-search-request-schema.json
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
title: ContactSearchRequest
---
