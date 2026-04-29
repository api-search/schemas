---
description: RetentionResult schema from Amplitude Dashboard REST API
layout: schema
name: RetentionResult
properties_list:
- description: Retention data organized by cohort date with day-by-day return percentages.
  name: data
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dashboard-rest-api-retention-result-schema.json
slug: dashboard-rest-api-retention-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-retention-result-schema.json\",\n  \"title\": \"RetentionResult\",\n  \"description\": \"RetentionResult schema from Amplitude Dashboard REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Retention data organized by cohort date with day-by-day return percentages.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-retention-result-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: RetentionResult
---
