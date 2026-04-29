---
description: Browser cookie object from a WebDriver session
layout: schema
name: Cookie
properties_list:
- description: Cookie name
  name: name
  type: string
- description: Cookie value
  name: value
  type: string
- description: Cookie domain
  name: domain
  type: string
- description: Cookie path
  name: path
  type: string
- description: Whether the cookie is HTTP-only
  name: httpOnly
  type: boolean
- description: Whether the cookie requires HTTPS
  name: secure
  type: boolean
- description: Cookie expiry as Unix timestamp
  name: expiry
  type: integer
provider_name: Appium
provider_slug: appium
schema_file: json-schema/appium-server-cookie-schema.json
slug: appium-server-cookie
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-cookie-schema.json\",\n  \"title\": \"Cookie\",\n  \"description\": \"Browser cookie object from a WebDriver session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie name\",\n      \"example\": \"session\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie value\",\n      \"example\": \"abc123\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie domain\",\n      \"example\": \"example.com\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie path\",\n      \"example\": \"/\"\n    },\n    \"httpOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cookie is HTTP-only\",\n      \"example\"\
  : false\n    },\n    \"secure\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cookie requires HTTPS\",\n      \"example\": false\n    },\n    \"expiry\": {\n      \"type\": \"integer\",\n      \"description\": \"Cookie expiry as Unix timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-cookie-schema.json
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
title: Cookie
---
