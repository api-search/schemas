---
description: A feature gate configuration that controls access to features based on targeting rules, conditions, and user properties. Feature gates are the core primitive for feature flagging in Statsig.
layout: schema
name: Statsig Feature Gate
properties_list:
- description: The unique identifier of the feature gate.
  name: id
  type: string
- description: The name of the feature gate, used as the key for SDK evaluation.
  name: name
  type: string
- description: A human-readable description of the gate's purpose and the feature it controls.
  name: description
  type: string
- description: Whether the gate is currently enabled and actively evaluating rules. When disabled, the gate returns false for all users.
  name: isEnabled
  type: boolean
- description: The current lifecycle status of the gate.
  name: status
  type: string
- description: The ordered list of targeting rules evaluated for this gate. Rules are evaluated top-to-bottom and the first matching rule determines the result.
  name: rules
  type: array
- description: ''
  name: overrides
  type: object
- description: Tags for organizing and categorizing the gate.
  name: tags
  type: array
- description: Target applications this gate is scoped to.
  name: targetApps
  type: array
- description: Salt value used for deterministic user assignment hashing.
  name: salt
  type: string
- description: Timestamp in milliseconds since epoch when the gate was created.
  name: createdTime
  type: integer
- description: Timestamp in milliseconds since epoch when the gate was last modified.
  name: lastModifiedTime
  type: integer
provider_name: statsig
provider_slug: statsig
schema_file: json-schema/statsig-feature-gate-schema.json
slug: statsig-feature-gate
source_filename: statsig-feature-gate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.statsig.com/schemas/statsig/feature-gate.json\",\n  \"title\": \"Statsig Feature Gate\",\n  \"description\": \"A feature gate configuration that controls access to features based on targeting rules, conditions, and user properties. Feature gates are the core primitive for feature flagging in Statsig.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the feature gate.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the feature gate, used as the key for SDK evaluation.\",\n      \"minLength\": 1,\n      \"maxLength\": 256,\n      \"pattern\": \"^[a-zA-Z0-9_\\\\-\\\\.]+$\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the gate's purpose and the\
  \ feature it controls.\",\n      \"maxLength\": 4096\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the gate is currently enabled and actively evaluating rules. When disabled, the gate returns false for all users.\",\n      \"default\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current lifecycle status of the gate.\",\n      \"enum\": [\"active\", \"disabled\", \"launched\", \"archived\"]\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"The ordered list of targeting rules evaluated for this gate. Rules are evaluated top-to-bottom and the first matching rule determines the result.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Rule\"\n      }\n    },\n    \"overrides\": {\n      \"$ref\": \"#/$defs/Overrides\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags for organizing and categorizing the gate.\",\n      \"items\": {\n\
  \        \"type\": \"string\"\n      }\n    },\n    \"targetApps\": {\n      \"type\": \"array\",\n      \"description\": \"Target applications this gate is scoped to.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"salt\": {\n      \"type\": \"string\",\n      \"description\": \"Salt value used for deterministic user assignment hashing.\"\n    },\n    \"createdTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp in milliseconds since epoch when the gate was created.\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp in milliseconds since epoch when the gate was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"Rule\": {\n      \"type\": \"object\",\n      \"description\": \"A targeting rule that defines conditions under which the gate passes or returns specific values.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"\
  The unique identifier of the rule.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable name for the rule.\"\n        },\n        \"passPercentage\": {\n          \"type\": \"number\",\n          \"description\": \"The percentage of users matching conditions who pass the rule.\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"default\": 100\n        },\n        \"conditions\": {\n          \"type\": \"array\",\n          \"description\": \"The conditions that must all be met for this rule to apply. Conditions within a rule are ANDed together.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Condition\"\n          }\n        },\n        \"returnValue\": {\n          \"type\": \"object\",\n          \"description\": \"The value returned when this rule matches, used for dynamic configs.\"\n        },\n        \"environments\": {\n          \"type\": \"array\",\n          \"description\": \"Environments\
  \ where this rule is active (e.g., production, staging).\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"Condition\": {\n      \"type\": \"object\",\n      \"description\": \"A condition within a targeting rule that evaluates user properties against specified criteria.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of condition to evaluate.\",\n          \"enum\": [\n            \"user_id\",\n            \"email\",\n            \"ip_address\",\n            \"country\",\n            \"app_version\",\n            \"custom_field\",\n            \"browser_name\",\n            \"browser_version\",\n            \"os_name\",\n            \"os_version\",\n            \"passes_gate\",\n            \"fails_gate\",\n            \"environment\",\n            \"passes_segment\",\n            \"fails_segment\",\n            \"time\",\n\
  \            \"unit_id\"\n          ]\n        },\n        \"targetValue\": {\n          \"description\": \"The value or array of values to compare against.\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator to use.\",\n          \"enum\": [\n            \"any\",\n            \"none\",\n            \"str_starts_with_any\",\n            \"str_ends_with_any\",\n            \"str_contains_any\",\n            \"str_contains_none\",\n            \"str_matches\",\n            \"gt\",\n            \"gte\",\n            \"lt\",\n            \"lte\",\n            \"version_gt\",\n            \"version_gte\",\n            \"version_lt\",\n            \"version_lte\",\n            \"before\",\n            \"after\",\n            \"on\"\n          ]\n        },\n        \"field\": {\n          \"type\": \"string\",\n          \"description\": \"The user field to evaluate, used with custom_field condition type.\"\n        }\n\
  \      }\n    },\n    \"Overrides\": {\n      \"type\": \"object\",\n      \"description\": \"User and ID overrides that force specific evaluation results, bypassing normal rule evaluation.\",\n      \"properties\": {\n        \"userOverrides\": {\n          \"type\": \"array\",\n          \"description\": \"User-specific overrides by user ID.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"userID\": {\n                \"type\": \"string\",\n                \"description\": \"The user ID to override.\"\n              },\n              \"value\": {\n                \"type\": \"boolean\",\n                \"description\": \"The forced evaluation result for this user.\"\n              }\n            },\n            \"required\": [\"userID\", \"value\"]\n          }\n        },\n        \"idOverrides\": {\n          \"type\": \"array\",\n          \"description\": \"ID-based overrides for custom ID types.\",\n          \"items\"\
  : {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ids\": {\n                \"type\": \"array\",\n                \"description\": \"The IDs to override.\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"value\": {\n                \"type\": \"boolean\",\n                \"description\": \"The forced evaluation result for these IDs.\"\n              }\n            },\n            \"required\": [\"ids\", \"value\"]\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/json-schema/statsig-feature-gate-schema.json
tags: []
title: Statsig Feature Gate
---
