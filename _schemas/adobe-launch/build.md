---
description: A build is the compiled output of a library. When a library is built, all of its resources (extensions, rules, and data elements) are compiled into a deployable artifact that is assigned to an environment for delivery. Builds represent the actual JavaScript or configuration files served to end users.
layout: schema
name: Adobe Experience Platform Tags Build
properties_list:
- description: The unique identifier for the build.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Related resources linked to this build.
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/build.json
slug: build
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/adobe-launch/json-schema/build.json\",\n  \"title\": \"Adobe Experience Platform Tags Build\",\n  \"description\": \"A build is the compiled output of a library. When a library is built, all of its resources (extensions, rules, and data elements) are compiled into a deployable artifact that is assigned to an environment for delivery. Builds represent the actual JavaScript or configuration files served to end users.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the build.\",\n      \"examples\": [\n        \"BL1234567890abcdef\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"builds\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"attributes\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pending\",\n            \"succeeded\",\n            \"failed\"\n          ],\n          \"description\": \"The current status of the build. Pending indicates the build is being compiled, succeeded means it is ready for deployment, and failed indicates a compilation error occurred.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"A unique token identifying this specific build artifact.\",\n          \"readOnly\": true\n        },\n        \"error_message\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The error message if the build failed. Null for successful builds.\",\n          \"readOnly\": true\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n         \
  \ \"description\": \"When the build was created (compilation started).\",\n          \"readOnly\": true\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the build status was last updated.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resources linked to this build.\",\n      \"properties\": {\n        \"library\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The library from which this build was compiled.\"\n        },\n        \"environment\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The environment where this build is deployed.\"\n        },\n        \"data_elements\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Data elements included in this build.\"\n        },\n        \"extensions\"\
  : {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Extensions included in this build.\"\n        },\n        \"rules\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Rules included in this build.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The canonical URL for this build resource.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"relationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"oneOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n          \
  \  {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"related\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/build.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: Adobe Experience Platform Tags Build
---
