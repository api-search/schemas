---
description: Measurement partner wrapping data for placements.
layout: schema
name: MeasurementPartnerWrappingData
properties_list:
- description: ''
  name: measurementPartner
  type: string
- description: ''
  name: tagWrappingMode
  type: string
- description: The wrapped tag content.
  name: wrappedTag
  type: string
- description: ''
  name: linkStatus
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-measurement-partner-wrapping-data-schema.json
slug: google-campaign-manager-measurement-partner-wrapping-data
source_filename: google-campaign-manager-measurement-partner-wrapping-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeasurementPartnerWrappingData\",\n  \"type\": \"object\",\n  \"description\": \"Measurement partner wrapping data for placements.\",\n  \"properties\": {\n    \"measurementPartner\": {\n      \"type\": \"string\"\n    },\n    \"tagWrappingMode\": {\n      \"type\": \"string\"\n    },\n    \"wrappedTag\": {\n      \"type\": \"string\",\n      \"description\": \"The wrapped tag content.\"\n    },\n    \"linkStatus\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-measurement-partner-wrapping-data-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: MeasurementPartnerWrappingData
---
