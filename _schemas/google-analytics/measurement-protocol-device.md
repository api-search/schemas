---
description: Device schema from Google Analytics API
layout: schema
name: Device
properties_list:
- description: Device category (e.g., mobile, tablet, desktop).
  name: category
  type: string
- description: Device language setting.
  name: language
  type: string
- description: Screen resolution (e.g., 1920x1080).
  name: screen_resolution
  type: string
- description: Operating system name.
  name: operating_system
  type: string
- description: Operating system version.
  name: operating_system_version
  type: string
- description: Device model.
  name: model
  type: string
- description: Device brand.
  name: brand
  type: string
- description: Browser name.
  name: browser
  type: string
- description: Browser version.
  name: browser_version
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/measurement-protocol-device-schema.json
slug: measurement-protocol-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"Device schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Device category (e.g., mobile, tablet, desktop).\",\n      \"example\": \"example_value\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Device language setting.\",\n      \"example\": \"example_value\"\n    },\n    \"screen_resolution\": {\n      \"type\": \"string\",\n      \"description\": \"Screen resolution (e.g., 1920x1080).\",\n      \"example\": \"example_value\"\n    },\n    \"operating_system\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system name.\",\n      \"example\": \"example_value\"\
  \n    },\n    \"operating_system_version\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system version.\",\n      \"example\": \"example_value\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Device model.\",\n      \"example\": \"example_value\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Device brand.\",\n      \"example\": \"example_value\"\n    },\n    \"browser\": {\n      \"type\": \"string\",\n      \"description\": \"Browser name.\",\n      \"example\": \"example_value\"\n    },\n    \"browser_version\": {\n      \"type\": \"string\",\n      \"description\": \"Browser version.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-device-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Device
---
