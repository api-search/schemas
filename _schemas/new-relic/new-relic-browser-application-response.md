---
description: ''
layout: schema
name: BrowserApplicationResponse
properties_list:
- description: ''
  name: browser_application
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-browser-application-response-schema.json
slug: new-relic-browser-application-response
source_filename: new-relic-browser-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"browser_application\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"browser_monitoring_key\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"loader_script\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserApplicationResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-browser-application-response-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: BrowserApplicationResponse
---
