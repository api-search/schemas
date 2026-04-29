---
description: Click-through URL configuration.
layout: schema
name: ClickThroughUrl
properties_list:
- description: Whether the campaign default landing page is used.
  name: defaultLandingPage
  type: boolean
- description: ID of the landing page for the click-through URL.
  name: landingPageId
  type: string
- description: Custom click-through URL.
  name: customClickThroughUrl
  type: string
- description: Read-only computed click-through URL. Set when either defaultLandingPage or landingPageId is set.
  name: computedClickThroughUrl
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-click-through-url-schema.json
slug: google-campaign-manager-click-through-url
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClickThroughUrl\",\n  \"type\": \"object\",\n  \"description\": \"Click-through URL configuration.\",\n  \"properties\": {\n    \"defaultLandingPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the campaign default landing page is used.\"\n    },\n    \"landingPageId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the landing page for the click-through URL.\"\n    },\n    \"customClickThroughUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Custom click-through URL.\"\n    },\n    \"computedClickThroughUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Read-only computed click-through URL. Set when either defaultLandingPage or landingPageId is set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-click-through-url-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ClickThroughUrl
---
