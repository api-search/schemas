---
description: SOAP response confirming the write operation. Returns the primary key of the affected record for insert operations.
layout: schema
name: WriteResponse
properties_list:
- description: Primary key of the created or modified record.
  name: primaryKey
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-write-response-schema.json
slug: adobe-campaign-classic-write-response
source_filename: adobe-campaign-classic-write-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-write-response-schema.json\",\n  \"title\": \"WriteResponse\",\n  \"description\": \"SOAP response confirming the write operation. Returns the primary key of the affected record for insert operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"primaryKey\": {\n      \"type\": \"string\",\n      \"description\": \"Primary key of the created or modified record.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-write-response-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: WriteResponse
---
