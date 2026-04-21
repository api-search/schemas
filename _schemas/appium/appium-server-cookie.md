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
