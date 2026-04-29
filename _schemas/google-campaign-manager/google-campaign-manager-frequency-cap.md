---
description: Frequency cap configuration.
layout: schema
name: FrequencyCap
properties_list:
- description: Number of times an individual user can be served the ad.
  name: impressions
  type: integer
- description: Duration of time, in seconds, for this frequency cap.
  name: duration
  type: integer
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-frequency-cap-schema.json
slug: google-campaign-manager-frequency-cap
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FrequencyCap\",\n  \"type\": \"object\",\n  \"description\": \"Frequency cap configuration.\",\n  \"properties\": {\n    \"impressions\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times an individual user can be served the ad.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of time, in seconds, for this frequency cap.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-frequency-cap-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: FrequencyCap
---
