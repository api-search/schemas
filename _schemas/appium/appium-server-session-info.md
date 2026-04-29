---
description: Information about a single active Appium session
layout: schema
name: SessionInfo
properties_list:
- description: Session identifier
  name: id
  type: string
- description: The capabilities used to create the session
  name: capabilities
  type: object
provider_name: Appium
provider_slug: appium
schema_file: json-schema/appium-server-session-info-schema.json
slug: appium-server-session-info
source_filename: appium-server-session-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-session-info-schema.json\",\n  \"title\": \"SessionInfo\",\n  \"description\": \"Information about a single active Appium session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Session identifier\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"The capabilities used to create the session\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-session-info-schema.json
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
title: SessionInfo
---
