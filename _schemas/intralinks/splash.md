---
description: A splash screen configuration for an Intralinks workspace, typically used to display NDA agreements, welcome messages, or branding to users entering the workspace.
layout: schema
name: Intralinks Splash Screen
properties_list:
- description: Unique identifier of the splash screen.
  name: id
  type: string
- description: Whether the splash screen requires user acceptance.
  name: hasAcceptButton
  type: boolean
- description: Text content of the splash screen.
  name: splashText
  type: string
- description: Whether the splash screen includes an image.
  name: hasImage
  type: boolean
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/splash.json
slug: splash
source_filename: splash.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"splash.json\",\n  \"title\": \"Intralinks Splash Screen\",\n  \"description\": \"A splash screen configuration for an Intralinks workspace, typically used to display NDA agreements, welcome messages, or branding to users entering the workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the splash screen.\"\n    },\n    \"hasAcceptButton\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the splash screen requires user acceptance.\"\n    },\n    \"splashText\": {\n      \"type\": \"string\",\n      \"description\": \"Text content of the splash screen.\"\n    },\n    \"hasImage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the splash screen includes an image.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/splash.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Splash Screen
---
