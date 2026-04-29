---
description: A rule in Adobe Experience Platform Tags controls resource behavior through a combination of events (triggers), conditions (criteria), and actions (executions). A rule belongs to exactly one property, and a property can have many rules. Rules are composed of rule components that define the specific logic.
layout: schema
name: Adobe Experience Platform Tags Rule
properties_list:
- description: The unique identifier for the rule.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Related resources linked to this rule.
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/rule.json
slug: rule
source_filename: rule.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/adobe-launch/json-schema/rule.json\",\n  \"title\": \"Adobe Experience Platform Tags Rule\",\n  \"description\": \"A rule in Adobe Experience Platform Tags controls resource behavior through a combination of events (triggers), conditions (criteria), and actions (executions). A rule belongs to exactly one property, and a property can have many rules. Rules are composed of rule components that define the specific logic.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the rule.\",\n      \"examples\": [\n        \"RL1234567890abcdef\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"rules\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"attributes\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable name of the rule.\",\n          \"minLength\": 1,\n          \"examples\": [\n            \"Page View Tracking Rule\",\n            \"Click Event Handler\"\n          ]\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether the rule is enabled and will be included in builds.\"\n        },\n        \"published\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the rule has been published to a production environment.\",\n          \"readOnly\": true\n        },\n        \"dirty\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the rule has unpublished changes since its last build.\",\n          \"readOnly\": true\n        },\n        \"revision_number\"\
  : {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The current revision number, incremented on each change.\",\n          \"readOnly\": true\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the rule was created.\",\n          \"readOnly\": true\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the rule was last updated.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resources linked to this rule.\",\n      \"properties\": {\n        \"property\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The property that owns this rule.\"\n        },\n        \"rule_components\": {\n          \"$ref\": \"#/$defs/relationship\",\n   \
  \       \"description\": \"The event, condition, and action components that make up this rule.\"\n        },\n        \"libraries\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Libraries that include this rule.\"\n        },\n        \"revisions\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Previous revisions of this rule.\"\n        },\n        \"origin\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The previous revision from which this rule was derived.\"\n        },\n        \"notes\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Notes associated with this rule.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The canonical URL for this rule resource.\"\n        }\n      }\n    }\n\
  \  },\n  \"$defs\": {\n    \"relationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"oneOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"related\": {\n              \"type\": \"string\"\
  ,\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/rule.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: Adobe Experience Platform Tags Rule
---
