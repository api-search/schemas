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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-action-sequence-schema.json\",\n  \"title\": \"ActionSequence\",\n  \"description\": \"A sequence of W3C Actions API input actions for a single input source\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pointer\",\n        \"key\",\n        \"wheel\",\n        \"none\"\n      ],\n      \"description\": \"The type of input source\",\n      \"example\": \"pointer\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this input source\",\n      \"example\": \"finger1\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Input source parameters\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"List of individual\
  \ action objects\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/json-schema/appium-server-action-sequence-schema.json
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
