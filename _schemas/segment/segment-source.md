---
description: A Segment source represents a data collection point that captures analytics events from a website, mobile app, server, or cloud application and sends them to Segment for routing to configured destinations.
layout: schema
name: Segment Source
properties_list:
- description: The unique identifier of the source.
  name: id
  type: string
- description: The URL-friendly slug of the source.
  name: slug
  type: string
- description: The display name of the source.
  name: name
  type: string
- description: Whether the source is currently enabled and collecting data.
  name: enabled
  type: boolean
- description: The write keys used to authenticate data sent to this source.
  name: writeKeys
  type: array
- description: ''
  name: metadata
  type: object
- description: Configuration settings specific to the source type.
  name: settings
  type: object
- description: Labels applied to the source for organization and access control.
  name: labels
  type: array
- description: The ID of the workspace this source belongs to.
  name: workspaceId
  type: string
provider_name: segment
provider_slug: segment
schema_file: json-schema/segment-source-schema.json
slug: segment-source
source_filename: segment-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://segment.com/schemas/segment/source.json\",\n  \"title\": \"Segment Source\",\n  \"description\": \"A Segment source represents a data collection point that captures analytics events from a website, mobile app, server, or cloud application and sends them to Segment for routing to configured destinations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"slug\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the source.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the source.\",\n      \"pattern\": \"^[a-z0-9-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the source.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the source is currently enabled and\
  \ collecting data.\"\n    },\n    \"writeKeys\": {\n      \"type\": \"array\",\n      \"description\": \"The write keys used to authenticate data sent to this source.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"minLength\": 1\n      }\n    },\n    \"metadata\": {\n      \"$ref\": \"#/$defs/SourceMetadata\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration settings specific to the source type.\",\n      \"additionalProperties\": true\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the source for organization and access control.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Label\"\n      }\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the workspace this source belongs to.\"\n    }\n  },\n  \"$defs\": {\n    \"SourceMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the source type\
  \ from the Segment catalog.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The metadata ID from the catalog.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the source type.\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"The slug of the source type.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the source type.\"\n        },\n        \"logos\": {\n          \"type\": \"object\",\n          \"description\": \"Logo URLs for the source.\",\n          \"properties\": {\n            \"default\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"Default logo URL.\"\n            }\n          }\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"description\"\
  : \"Categories the source belongs to.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"Label\": {\n      \"type\": \"object\",\n      \"description\": \"A label used to organize and control access to workspace resources.\",\n      \"required\": [\"key\", \"value\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The label key.\",\n          \"minLength\": 1\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The label value.\",\n          \"minLength\": 1\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the label.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/json-schema/segment-source-schema.json
tags: []
title: Segment Source
---
