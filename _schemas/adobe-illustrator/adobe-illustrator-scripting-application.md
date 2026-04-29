---
description: Application from Adobe Illustrator API
layout: schema
name: Application
properties_list:
- description: The application name.
  name: name
  type: string
- description: The version string.
  name: version
  type: string
- description: The build number.
  name: buildNumber
  type: string
- description: The current locale.
  name: locale
  type: string
- description: The scripting API version.
  name: scriptingVersion
  type: string
- description: Available memory in bytes.
  name: freeMemory
  type: integer
- description: Name of the currently active document.
  name: activeDocument
  type: string
- description: List of open document names.
  name: documents
  type: array
- description: The level of user interaction allowed.
  name: userInteractionLevel
  type: string
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-application-schema.json
slug: adobe-illustrator-scripting-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"Application from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The application name.\",\n      \"examples\": [\n        \"Adobe Illustrator\"\n      ],\n      \"example\": \"Example Artboard\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version string.\",\n      \"examples\": [\n        29.0\n      ],\n      \"example\": \"example_value\"\n    },\n    \"buildNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The build number.\",\n      \"example\": \"example_value\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The current locale.\",\n      \"examples\": [\n        \"en_US\"\n      ],\n      \"example\": \"example_value\"\n    },\n    \"scriptingVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The scripting API version.\",\n      \"example\": \"example_value\"\n    },\n    \"freeMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"Available memory in bytes.\",\n      \"example\": 1024\n    },\n    \"activeDocument\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the currently active document.\",\n      \"example\": \"example_value\"\n    },\n    \"documents\": {\n      \"type\": \"array\",\n      \"description\": \"List of open document names.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userInteractionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The level of user interaction allowed.\",\n      \"enum\": [\n        \"DISPLAYALERTS\",\n        \"DONTDISPLAYALERTS\"\n      ],\n      \"\
  example\": \"DISPLAYALERTS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-application-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: Application
---
