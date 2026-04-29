---
description: Represents a Google Tag Manager Parameter. Parameters are key-value pairs that configure tags, triggers, and variables.
layout: schema
name: Parameter
properties_list:
- description: The parameter type.
  name: type
  type: string
- description: The named key that uniquely identifies a parameter. Required for top-level parameters, as well as map values. Ignored for list values.
  name: key
  type: string
- description: A parameter's value (may contain variable references) as appropriate to the specified type.
  name: value
  type: string
- description: This list parameter's parameters (keys will be ignored). Used when type is list.
  name: list
  type: array
- description: This map parameter's parameters (must have keys; keys must be unique). Used when type is map.
  name: map
  type: array
- description: Whether or not the parameter is a weak reference. Used to determine which parameters should be included in exported containers.
  name: isWeakReference
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-parameter-schema.json
slug: google-tag-manager-v2-parameter
source_filename: google-tag-manager-v2-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parameter\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Google Tag Manager Parameter. Parameters are key-value pairs that configure tags, triggers, and variables.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter type.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The named key that uniquely identifies a parameter. Required for top-level parameters, as well as map values. Ignored for list values.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"A parameter's value (may contain variable references) as appropriate to the specified type.\"\n    },\n    \"list\": {\n      \"type\": \"array\",\n      \"description\": \"This list parameter's parameters (keys will be ignored). Used when type is list.\"\n    },\n    \"map\": {\n      \"type\": \"array\",\n\
  \      \"description\": \"This map parameter's parameters (must have keys; keys must be unique). Used when type is map.\"\n    },\n    \"isWeakReference\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not the parameter is a weak reference. Used to determine which parameters should be included in exported containers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-parameter-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: Parameter
---
