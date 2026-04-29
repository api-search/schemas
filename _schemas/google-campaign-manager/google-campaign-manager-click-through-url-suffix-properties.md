---
description: Click-through URL suffix properties.
layout: schema
name: ClickThroughUrlSuffixProperties
properties_list:
- description: Click-through URL suffix to apply to all ads in this entity's scope.
  name: clickThroughUrlSuffix
  type: string
- description: Whether this entity should override the inherited suffix with its own defined suffix.
  name: overrideInheritedSuffix
  type: boolean
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-click-through-url-suffix-properties-schema.json
slug: google-campaign-manager-click-through-url-suffix-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClickThroughUrlSuffixProperties\",\n  \"type\": \"object\",\n  \"description\": \"Click-through URL suffix properties.\",\n  \"properties\": {\n    \"clickThroughUrlSuffix\": {\n      \"type\": \"string\",\n      \"description\": \"Click-through URL suffix to apply to all ads in this entity's scope.\"\n    },\n    \"overrideInheritedSuffix\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this entity should override the inherited suffix with its own defined suffix.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-click-through-url-suffix-properties-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ClickThroughUrlSuffixProperties
---
