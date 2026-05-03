---
description: A Segment destination represents a configured integration that receives analytics data routed from Segment sources. Destinations can be analytics tools, data warehouses, marketing platforms, or custom webhook endpoints.
layout: schema
name: Segment Destination
properties_list:
- description: The unique identifier of the destination.
  name: id
  type: string
- description: The display name of the destination.
  name: name
  type: string
- description: Whether the destination is currently enabled and receiving data.
  name: enabled
  type: boolean
- description: The ID of the source this destination is connected to.
  name: sourceId
  type: string
- description: ''
  name: metadata
  type: object
- description: Configuration settings specific to the destination type, such as API keys, account IDs, or mapping options.
  name: settings
  type: object
- description: Labels applied to the destination for organization and access control.
  name: labels
  type: array
provider_name: segment
provider_slug: segment
schema_file: json-schema/segment-destination-schema.json
slug: segment-destination
source_filename: segment-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://segment.com/schemas/segment/destination.json\",\n  \"title\": \"Segment Destination\",\n  \"description\": \"A Segment destination represents a configured integration that receives analytics data routed from Segment sources. Destinations can be analytics tools, data warehouses, marketing platforms, or custom webhook endpoints.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the destination.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the destination.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the destination is currently enabled and receiving data.\"\n    },\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the source this\
  \ destination is connected to.\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/$defs/DestinationMetadata\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration settings specific to the destination type, such as API keys, account IDs, or mapping options.\",\n      \"additionalProperties\": true\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the destination for organization and access control.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"key\", \"value\"],\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The label key.\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The label value.\"\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"DestinationMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"\
  Metadata about the destination type from the Segment catalog.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The metadata ID from the catalog.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the destination integration.\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"The slug of the destination integration.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the destination integration.\"\n        },\n        \"logos\": {\n          \"type\": \"object\",\n          \"description\": \"Logo URLs for the destination.\",\n          \"properties\": {\n            \"default\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"Default logo URL.\"\n            }\n          }\n        },\n      \
  \  \"categories\": {\n          \"type\": \"array\",\n          \"description\": \"Categories the destination belongs to.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"supportedMethods\": {\n          \"type\": \"object\",\n          \"description\": \"Which Segment call types this destination supports.\",\n          \"properties\": {\n            \"track\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether track calls are supported.\"\n            },\n            \"identify\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether identify calls are supported.\"\n            },\n            \"page\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether page calls are supported.\"\n            },\n            \"screen\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether screen calls are supported.\"\n            },\n\
  \            \"group\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether group calls are supported.\"\n            },\n            \"alias\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether alias calls are supported.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/json-schema/segment-destination-schema.json
tags: []
title: Segment Destination
---
