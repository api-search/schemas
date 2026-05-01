---
description: Webvtt Destination Settings
layout: schema
name: WebvttDestinationSettings
properties_list:
- description: ''
  name: StyleControl
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-webvtt-destination-settings-schema.json
slug: medialive-api-webvtt-destination-settings
source_filename: medialive-api-webvtt-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-webvtt-destination-settings-schema.json\",\n  \"title\": \"WebvttDestinationSettings\",\n  \"description\": \"Webvtt Destination Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StyleControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebvttDestinationStyleControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"styleControl\"\n          },\n          \"description\": \"Controls whether the color and position of the source captions is passed through to the WebVTT output captions.  PASSTHROUGH - Valid only if the source captions are EMBEDDED or TELETEXT.  NO_STYLE_DATA - Don't pass through the style. The output captions will not contain any font styling information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-webvtt-destination-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: WebvttDestinationSettings
---
