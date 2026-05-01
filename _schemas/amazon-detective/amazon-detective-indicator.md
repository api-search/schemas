---
description: An indicator of compromise detected during an investigation
layout: schema
name: Indicator
properties_list:
- description: The type of indicator.
  name: IndicatorType
  type: string
- description: Details about the indicator of compromise.
  name: IndicatorDetail
  type: object
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-indicator-schema.json
slug: amazon-detective-indicator
source_filename: amazon-detective-indicator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-indicator-schema.json\",\n  \"title\": \"Indicator\",\n  \"description\": \"An indicator of compromise detected during an investigation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IndicatorType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of indicator.\",\n      \"enum\": [\n        \"TTP_OBSERVED\",\n        \"IMPOSSIBLE_TRAVEL\",\n        \"FLAGGED_IP_ADDRESS\",\n        \"NEW_GEOLOCATION\",\n        \"NEW_ASO\",\n        \"NEW_USER_AGENT\",\n        \"RELATED_FINDING\",\n        \"RELATED_FINDING_GROUP\"\n      ],\n      \"example\": \"FLAGGED_IP_ADDRESS\"\n    },\n    \"IndicatorDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the indicator of compromise.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-indicator-schema.json
tags:
- Forensics
- Investigation
- Security
title: Indicator
---
