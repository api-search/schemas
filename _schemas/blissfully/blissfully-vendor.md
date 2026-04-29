---
description: A software vendor in the Vendr catalog
layout: schema
name: Vendor
properties_list:
- description: Unique vendor identifier
  name: id
  type: string
- description: Vendor name
  name: name
  type: string
- description: Vendor website URL
  name: website
  type: string
- description: Primary product category
  name: category
  type: string
provider_name: Blissfully
provider_slug: blissfully
schema_file: json-schema/blissfully-vendor-schema.json
slug: blissfully-vendor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-vendor-schema.json\",\n  \"title\": \"Vendor\",\n  \"description\": \"A software vendor in the Vendr catalog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique vendor identifier\",\n      \"example\": \"vendor-salesforce\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor name\",\n      \"example\": \"Salesforce\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Vendor website URL\",\n      \"example\": \"https://www.salesforce.com\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Primary product category\",\n      \"example\": \"CRM\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-vendor-schema.json
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
title: Vendor
---
