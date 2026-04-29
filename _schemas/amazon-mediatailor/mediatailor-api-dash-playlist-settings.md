---
description: Dash manifest configuration parameters.
layout: schema
name: DashPlaylistSettings
properties_list:
- description: ''
  name: ManifestWindowSeconds
  type: object
- description: ''
  name: MinBufferTimeSeconds
  type: object
- description: ''
  name: MinUpdatePeriodSeconds
  type: object
- description: ''
  name: SuggestedPresentationDelaySeconds
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-dash-playlist-settings-schema.json
slug: mediatailor-api-dash-playlist-settings
source_filename: mediatailor-api-dash-playlist-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-dash-playlist-settings-schema.json\",\n  \"title\": \"DashPlaylistSettings\",\n  \"description\": \"Dash manifest configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManifestWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total duration (in seconds) of each manifest. Minimum value: <code>30</code> seconds. Maximum value: <code>3600</code> seconds.\"\n        }\n      ]\n    },\n    \"MinBufferTimeSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Minimum amount of content (measured in seconds) that a player must keep available in the buffer.\
  \ Minimum value: <code>2</code> seconds. Maximum value: <code>60</code> seconds.\"\n        }\n      ]\n    },\n    \"MinUpdatePeriodSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Minimum amount of time (in seconds) that the player should wait before requesting updates to the manifest. Minimum value: <code>2</code> seconds. Maximum value: <code>60</code> seconds.\"\n        }\n      ]\n    },\n    \"SuggestedPresentationDelaySeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Amount of time (in seconds) that the player should be from the live point at the end of the manifest. Minimum value: <code>2</code> seconds. Maximum value: <code>60</code> seconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-dash-playlist-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashPlaylistSettings
---
