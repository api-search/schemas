---
description: Ad blocking configuration for a campaign.
layout: schema
name: AdBlockingConfiguration
properties_list:
- description: Whether this campaign has enabled ad blocking. When true, ad blocking is enabled for the campaign and a default ad can be served for blocked ads.
  name: enabled
  type: boolean
- description: Override click-through URL for blocked ads.
  name: overrideClickThroughUrl
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-ad-blocking-configuration-schema.json
slug: google-campaign-manager-ad-blocking-configuration
source_filename: google-campaign-manager-ad-blocking-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AdBlockingConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Ad blocking configuration for a campaign.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this campaign has enabled ad blocking. When true, ad blocking is enabled for the campaign and a default ad can be served for blocked ads.\"\n    },\n    \"overrideClickThroughUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Override click-through URL for blocked ads.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-ad-blocking-configuration-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: AdBlockingConfiguration
---
