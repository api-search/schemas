---
description: A library is a collection of tag resources (extensions, rules, and data elements) that are compiled together into a build for deployment. Libraries follow a publishing workflow from development through staging to production, and serve as the mechanism for testing and deploying tag configurations.
layout: schema
name: Adobe Experience Platform Tags Library
properties_list:
- description: The unique identifier for the library.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Related resources linked to this library.
  name: relationships
  type: object
- description: ''
  name: links
  type: object
- description: Metadata for library state transitions.
  name: meta
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/library.json
slug: library
source_filename: library.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/adobe-launch/json-schema/library.json\",\n  \"title\": \"Adobe Experience Platform Tags Library\",\n  \"description\": \"A library is a collection of tag resources (extensions, rules, and data elements) that are compiled together into a build for deployment. Libraries follow a publishing workflow from development through staging to production, and serve as the mechanism for testing and deploying tag configurations.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the library.\",\n      \"examples\": [\n        \"LB1234567890abcdef\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"libraries\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"attributes\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable name of the library.\",\n          \"minLength\": 1,\n          \"examples\": [\n            \"Q1 2026 Release\",\n            \"Analytics Update v2\"\n          ]\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"development\",\n            \"submitted\",\n            \"approved\",\n            \"rejected\",\n            \"published\"\n          ],\n          \"default\": \"development\",\n          \"description\": \"The current publishing state of the library. Libraries progress through: development -> submitted -> approved -> published, or can be rejected back to development.\"\n        },\n        \"build_required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the library has changes that\
  \ require a new build before deployment.\",\n          \"readOnly\": true\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the library was created.\",\n          \"readOnly\": true\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the library was last updated.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resources linked to this library.\",\n      \"properties\": {\n        \"property\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The property that owns this library.\"\n        },\n        \"environment\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The environment to which this library is assigned for deployment.\"\n        },\n\
  \        \"data_elements\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Data elements included in this library.\"\n        },\n        \"extensions\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Extensions included in this library.\"\n        },\n        \"rules\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Rules included in this library.\"\n        },\n        \"builds\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Builds compiled from this library.\"\n        },\n        \"last_build\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The most recent build compiled from this library.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The canonical URL\
  \ for this library resource.\"\n        }\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for library state transitions.\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"submit\",\n            \"approve\",\n            \"reject\",\n            \"develop\"\n          ],\n          \"description\": \"The publishing workflow transition to perform: submit (development -> submitted), approve (submitted -> approved), reject (submitted/approved -> development), develop (move back to development).\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"relationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"oneOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n    \
  \              \"type\": \"string\"\n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"related\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/library.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: Adobe Experience Platform Tags Library
---
