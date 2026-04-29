---
description: Request body identifying an app by package name or bundle ID
layout: schema
name: AppIdRequest
properties_list:
- description: App package name (Android) or bundle ID (iOS)
  name: appId
  type: string
- description: iOS bundle identifier
  name: bundleId
  type: string
- description: Platform-specific options
  name: options
  type: object
provider_name: Appium
provider_slug: appium
schema_file: json-schema/appium-server-app-id-request-schema.json
slug: appium-server-app-id-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-app-id-request-schema.json\",\n  \"title\": \"AppIdRequest\",\n  \"description\": \"Request body identifying an app by package name or bundle ID\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"App package name (Android) or bundle ID (iOS)\",\n      \"example\": \"com.example.app\"\n    },\n    \"bundleId\": {\n      \"type\": \"string\",\n      \"description\": \"iOS bundle identifier\",\n      \"example\": \"com.example.app\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Platform-specific options\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-app-id-request-schema.json
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
title: AppIdRequest
---
