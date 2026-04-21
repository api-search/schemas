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
