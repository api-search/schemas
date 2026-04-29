---
description: A field value with display metadata
layout: schema
name: FieldValueRepresentation
properties_list:
- description: Human-readable formatted display value (for dates, picklists, lookups)
  name: displayValue
  type: object
- description: Raw field value
  name: value
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-field-value-representation-schema.json
slug: salesforce-ui-field-value-representation
source_filename: salesforce-ui-field-value-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A field value with display metadata\",\n  \"properties\": {\n    \"displayValue\": {\n      \"type\": \"object\",\n      \"description\": \"Human-readable formatted display value (for dates, picklists, lookups)\",\n      \"example\": \"example_value\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"Raw field value\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldValueRepresentation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-field-value-representation-schema.json
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
title: FieldValueRepresentation
---
