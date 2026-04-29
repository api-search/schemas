---
description: A vendor or subcontractor record.
layout: schema
name: Vendor
properties_list:
- description: Vendor identifier.
  name: id
  type: string
- description: Vendor name.
  name: name
  type: string
- description: Primary vendor contact email.
  name: email
  type: string
- description: Vendor phone number.
  name: phone
  type: string
- description: Vendor address.
  name: address
  type: string
- description: Vendor tax identification number.
  name: tax_id
  type: string
- description: Vendor status.
  name: status
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-vendor-schema.json
slug: unified-api-vendor
source_filename: unified-api-vendor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-vendor-schema.json\",\n  \"title\": \"Vendor\",\n  \"description\": \"A vendor or subcontractor record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor identifier.\",\n      \"example\": \"ven-334455\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor name.\",\n      \"example\": \"ABC Concrete Contractors\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Primary vendor contact email.\",\n      \"example\": \"admin@abcconcrete.com\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor phone number.\",\n      \"example\": 14155551234\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor\
  \ address.\",\n      \"example\": \"456 Industrial Blvd, Oakland, CA 94601\"\n    },\n    \"tax_id\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor tax identification number.\",\n      \"example\": \"12-3456789\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-vendor-schema.json
tags:
- Accounting
- Construction
- Integration
title: Vendor
---
