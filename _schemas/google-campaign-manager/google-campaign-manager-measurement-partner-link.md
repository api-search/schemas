---
description: Measurement partner integration link.
layout: schema
name: MeasurementPartnerLink
properties_list:
- description: Measurement partner used for tag wrapping.
  name: measurementPartner
  type: string
- description: The status of the link.
  name: linkStatus
  type: string
- description: Partner campaign ID for the link.
  name: partnerCampaignId
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-measurement-partner-link-schema.json
slug: google-campaign-manager-measurement-partner-link
source_filename: google-campaign-manager-measurement-partner-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeasurementPartnerLink\",\n  \"type\": \"object\",\n  \"description\": \"Measurement partner integration link.\",\n  \"properties\": {\n    \"measurementPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Measurement partner used for tag wrapping.\"\n    },\n    \"linkStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the link.\"\n    },\n    \"partnerCampaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Partner campaign ID for the link.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-measurement-partner-link-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: MeasurementPartnerLink
---
