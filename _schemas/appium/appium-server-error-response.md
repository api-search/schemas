---
description: WebDriver protocol error response
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: value
  type: object
provider_name: Appium
provider_slug: appium
schema_file: json-schema/appium-server-error-response-schema.json
slug: appium-server-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"WebDriver protocol error response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"Error code\",\n          \"example\": \"no such element\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable error message\",\n          \"example\": \"An element could not be located on the page using the given search parameters.\"\n        },\n        \"stacktrace\": {\n          \"type\": \"string\",\n          \"description\": \"Stack trace for debugging\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-error-response-schema.json
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
title: ErrorResponse
---
