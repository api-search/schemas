---
description: Preferences from Adobe Illustrator API
layout: schema
name: Preferences
properties_list:
- description: Default ruler units.
  name: rulerUnits
  type: string
- description: ''
  name: generalPreferences
  type: object
- description: ''
  name: typePreferences
  type: object
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
schema_file: json-schema/adobe-illustrator-scripting-preferences-schema.json
slug: adobe-illustrator-scripting-preferences
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-preferences-schema.json\",\n  \"title\": \"Preferences\",\n  \"description\": \"Preferences from Adobe Illustrator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rulerUnits\": {\n      \"type\": \"string\",\n      \"description\": \"Default ruler units.\",\n      \"enum\": [\n        \"Points\",\n        \"Picas\",\n        \"Inches\",\n        \"Millimeters\",\n        \"Centimeters\",\n        \"Pixels\"\n      ],\n      \"example\": \"Points\"\n    },\n    \"generalPreferences\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"keyboardIncrement\": {\n          \"type\": \"number\",\n          \"description\": \"Keyboard increment value.\"\n        },\n        \"constrainAngle\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"Constrain angle in degrees.\"\n        },\n        \"useAreaSelect\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use area select.\"\n        }\n      }\n    },\n    \"typePreferences\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"showHiddenCharacters\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to show hidden characters.\"\n        },\n        \"useSmartQuotes\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use smart quotes.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/json-schema/adobe-illustrator-scripting-preferences-schema.json
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
title: Preferences
---
