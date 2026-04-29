---
description: FunnelResult schema from Amplitude Dashboard REST API
layout: schema
name: FunnelResult
properties_list:
- description: Funnel conversion data including step-by-step drop-off rates.
  name: data
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dashboard-rest-api-funnel-result-schema.json
slug: dashboard-rest-api-funnel-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-funnel-result-schema.json\",\n  \"title\": \"FunnelResult\",\n  \"description\": \"FunnelResult schema from Amplitude Dashboard REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Funnel conversion data including step-by-step drop-off rates.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-funnel-result-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: FunnelResult
---
