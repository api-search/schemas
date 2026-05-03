---
description: Schema representing a feature flag in Optimizely Feature Experimentation, including variables, variations, and environment-specific rulesets for controlled rollouts and experimentation.
layout: schema
name: Optimizely Feature Flag
properties_list:
- description: Unique key for the feature flag used in SDK code
  name: key
  type: string
- description: Human-readable name of the feature flag
  name: name
  type: string
- description: Description of the flag's purpose and behavior
  name: description
  type: string
- description: The project this flag belongs to
  name: project_id
  type: integer
- description: Remote configuration variables that can be set per variation
  name: variables
  type: array
- description: Variations of the flag with different variable values
  name: variations
  type: array
- description: Per-environment flag configurations with rulesets
  name: environments
  type: object
- description: Timestamp when the flag was created
  name: created
  type: string
- description: Timestamp when the flag was last modified
  name: last_modified
  type: string
provider_name: Optimizely
provider_slug: optimizely
schema_file: json-schema/optimizely-feature-flag-schema.json
slug: optimizely-feature-flag
source_filename: optimizely-feature-flag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.optimizely.com/schemas/optimizely/feature-flag.json\",\n  \"title\": \"Optimizely Feature Flag\",\n  \"description\": \"Schema representing a feature flag in Optimizely Feature Experimentation, including variables, variations, and environment-specific rulesets for controlled rollouts and experimentation.\",\n  \"type\": \"object\",\n  \"required\": [\"key\", \"name\"],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique key for the feature flag used in SDK code\",\n      \"minLength\": 1,\n      \"maxLength\": 64,\n      \"pattern\": \"^[a-z0-9_]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the feature flag\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the flag's purpose\
  \ and behavior\",\n      \"maxLength\": 2000\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The project this flag belongs to\"\n    },\n    \"variables\": {\n      \"type\": \"array\",\n      \"description\": \"Remote configuration variables that can be set per variation\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Variable\"\n      }\n    },\n    \"variations\": {\n      \"type\": \"array\",\n      \"description\": \"Variations of the flag with different variable values\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FlagVariation\"\n      }\n    },\n    \"environments\": {\n      \"type\": \"object\",\n      \"description\": \"Per-environment flag configurations with rulesets\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/FlagEnvironment\"\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the flag was created\"\n    },\n   \
  \ \"last_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the flag was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Variable\": {\n      \"type\": \"object\",\n      \"description\": \"A remotely configurable variable within a feature flag\",\n      \"required\": [\"key\", \"type\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Unique key for the variable\",\n          \"minLength\": 1,\n          \"pattern\": \"^[a-z0-9_]+$\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of the variable\",\n          \"enum\": [\"string\", \"integer\", \"double\", \"boolean\", \"json\"]\n        },\n        \"default_value\": {\n          \"type\": \"string\",\n          \"description\": \"Default value of the variable when no variation overrides it\"\n        }\n      }\n    },\n    \"FlagVariation\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"A variation of a feature flag with specific variable values\",\n      \"required\": [\"key\", \"name\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Unique key for the variation\",\n          \"minLength\": 1,\n          \"pattern\": \"^[a-z0-9_]+$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the variation\"\n        },\n        \"variables\": {\n          \"type\": \"object\",\n          \"description\": \"Variable key-value overrides for this variation\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"FlagEnvironment\": {\n      \"type\": \"object\",\n      \"description\": \"Flag configuration for a specific environment\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"\
  description\": \"Whether the flag is enabled in this environment\"\n        },\n        \"ruleset\": {\n          \"$ref\": \"#/$defs/Ruleset\"\n        }\n      }\n    },\n    \"Ruleset\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of rules determining flag behavior in an environment\",\n      \"properties\": {\n        \"rules\": {\n          \"type\": \"array\",\n          \"description\": \"Ordered list of rules evaluated top-to-bottom\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Rule\"\n          }\n        }\n      }\n    },\n    \"Rule\": {\n      \"type\": \"object\",\n      \"description\": \"A rule that determines which variation to deliver to matching visitors\",\n      \"required\": [\"key\", \"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the rule\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\":\
  \ \"Unique key for the rule\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of delivery rule\",\n          \"enum\": [\"a/b_test\", \"targeted_delivery\", \"personalization\"]\n        },\n        \"audience_conditions\": {\n          \"type\": \"string\",\n          \"description\": \"JSON-encoded audience targeting conditions\"\n        },\n        \"percentage_included\": {\n          \"type\": \"integer\",\n          \"description\": \"Percentage of matching traffic included in this rule\",\n          \"minimum\": 0,\n          \"maximum\": 10000\n        },\n        \"variations\": {\n          \"type\": \"array\",\n          \"description\": \"Variation allocation within the rule\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"variation_key\": {\n                \"type\": \"string\",\n                \"description\": \"Key of the variation\"\n              },\n   \
  \           \"weight\": {\n                \"type\": \"integer\",\n                \"description\": \"Traffic weight allocation\",\n                \"minimum\": 0,\n                \"maximum\": 10000\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/json-schema/optimizely-feature-flag-schema.json
tags:
- A/B Testing
- Content Management
- Customer Data
- E-Commerce
- Experimentation
- Feature Flags
- Marketing
title: Optimizely Feature Flag
---
