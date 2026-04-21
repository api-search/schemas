---
description: A sequence of W3C Actions API input actions for a single input source
layout: schema
name: ActionSequence
properties_list:
- description: The type of input source
  name: type
  type: string
- description: Unique identifier for this input source
  name: id
  type: string
- description: Input source parameters
  name: parameters
  type: object
- description: List of individual action objects
  name: actions
  type: array
provider_name: Appium
provider_slug: appium
schema_file: json-schema/appium-server-action-sequence-schema.json
slug: appium-server-action-sequence
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
title: ActionSequence
---
