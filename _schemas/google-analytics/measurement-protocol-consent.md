---
description: Consent schema from Google Analytics API
layout: schema
name: Consent
properties_list:
- description: Consent for using user data in advertising.
  name: ad_user_data
  type: string
- description: Consent for ad personalization.
  name: ad_personalization
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/measurement-protocol-consent-schema.json
slug: measurement-protocol-consent
source_filename: measurement-protocol-consent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-consent-schema.json\",\n  \"title\": \"Consent\",\n  \"description\": \"Consent schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ad_user_data\": {\n      \"type\": \"string\",\n      \"description\": \"Consent for using user data in advertising.\",\n      \"enum\": [\n        \"GRANTED\",\n        \"DENIED\"\n      ],\n      \"example\": \"GRANTED\"\n    },\n    \"ad_personalization\": {\n      \"type\": \"string\",\n      \"description\": \"Consent for ad personalization.\",\n      \"enum\": [\n        \"GRANTED\",\n        \"DENIED\"\n      ],\n      \"example\": \"GRANTED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-consent-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Consent
---
