---
description: Lookback window configuration for attribution.
layout: schema
name: LookbackConfiguration
properties_list:
- description: Lookback window, in days, from the last time a given user clicked on one of your ads.
  name: clickDuration
  type: integer
- description: Lookback window, in days, from the last time a given user viewed one of your ads.
  name: postImpressionActivitiesDuration
  type: integer
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-lookback-configuration-schema.json
slug: google-campaign-manager-lookback-configuration
source_filename: google-campaign-manager-lookback-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LookbackConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Lookback window configuration for attribution.\",\n  \"properties\": {\n    \"clickDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Lookback window, in days, from the last time a given user clicked on one of your ads.\"\n    },\n    \"postImpressionActivitiesDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Lookback window, in days, from the last time a given user viewed one of your ads.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-lookback-configuration-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: LookbackConfiguration
---
