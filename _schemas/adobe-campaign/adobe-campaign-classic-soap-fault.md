---
description: SOAP fault response indicating an error during operation processing.
layout: schema
name: SOAPFault
properties_list:
- description: Fault code identifying the error category.
  name: faultcode
  type: string
- description: Human-readable description of the error.
  name: faultstring
  type: string
- description: Additional error details.
  name: detail
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-soap-fault-schema.json
slug: adobe-campaign-classic-soap-fault
source_filename: adobe-campaign-classic-soap-fault-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-soap-fault-schema.json\",\n  \"title\": \"SOAPFault\",\n  \"description\": \"SOAP fault response indicating an error during operation processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"faultcode\": {\n      \"type\": \"string\",\n      \"description\": \"Fault code identifying the error category.\",\n      \"example\": \"example_value\"\n    },\n    \"faultstring\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the error.\",\n      \"example\": \"example_value\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Additional error details.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-soap-fault-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: SOAPFault
---
