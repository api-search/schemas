---
description: Request to find an element using a locator strategy
layout: schema
name: FindElementRequest
properties_list:
- description: The element locator strategy
  name: using
  type: string
- description: The selector value for the locator strategy
  name: value
  type: string
provider_name: Appium
provider_slug: appium
schema_file: json-schema/appium-server-find-element-request-schema.json
slug: appium-server-find-element-request
source_filename: appium-server-find-element-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-find-element-request-schema.json\",\n  \"title\": \"FindElementRequest\",\n  \"description\": \"Request to find an element using a locator strategy\",\n  \"type\": \"object\",\n  \"required\": [\n    \"using\",\n    \"value\"\n  ],\n  \"properties\": {\n    \"using\": {\n      \"type\": \"string\",\n      \"description\": \"The element locator strategy\",\n      \"enum\": [\n        \"accessibility id\",\n        \"id\",\n        \"xpath\",\n        \"class name\",\n        \"name\",\n        \"css selector\",\n        \"-android uiautomator\",\n        \"-ios predicate string\"\n      ],\n      \"example\": \"accessibility id\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The selector value for the locator strategy\",\n      \"example\": \"Login Button\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-find-element-request-schema.json
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
title: FindElementRequest
---
