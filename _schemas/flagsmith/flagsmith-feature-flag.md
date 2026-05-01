---
description: A feature flag definition in Flagsmith including its metadata, type, default configuration, and multivariate options. Feature flags are the core primitive in Flagsmith for controlling feature rollouts and remote configuration.
layout: schema
name: Flagsmith Feature Flag
properties_list:
- description: The unique identifier for this feature flag
  name: id
  type: integer
- description: The name of the feature flag, used as the key in SDK lookups
  name: name
  type: string
- description: A human-readable description of the feature flag and its purpose
  name: description
  type:
  - string
  - 'null'
- description: The date and time the feature flag was created
  name: created_date
  type: string
- description: The initial value assigned to the feature when it was created
  name: initial_value
  type:
  - string
  - 'null'
- description: Whether the feature flag is enabled by default in new environments
  name: default_enabled
  type: boolean
- description: The type of feature flag. STANDARD for simple on/off flags with an optional value, MULTIVARIATE for flags with multiple weighted value variations
  name: type
  type: string
- description: The ID of the project this feature flag belongs to
  name: project
  type: integer
- description: Whether the feature flag is archived and hidden from the dashboard by default
  name: is_archived
  type: boolean
- description: The users who are designated as owners of this feature flag
  name: owners
  type: array
- description: The IDs of tags associated with this feature flag for organization
  name: tags
  type: array
- description: The multivariate value options available for this feature flag when the type is MULTIVARIATE
  name: multivariate_options
  type: array
provider_name: flagsmith
provider_slug: flagsmith
schema_file: json-schema/flagsmith-feature-flag-schema.json
slug: flagsmith-feature-flag
source_filename: flagsmith-feature-flag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://flagsmith.com/schemas/flagsmith/feature-flag.json\",\n  \"title\": \"Flagsmith Feature Flag\",\n  \"description\": \"A feature flag definition in Flagsmith including its metadata, type, default configuration, and multivariate options. Feature flags are the core primitive in Flagsmith for controlling feature rollouts and remote configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for this feature flag\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the feature flag, used as the key in SDK lookups\",\n      \"pattern\": \"^[-_.a-zA-Z0-9]+$\",\n      \"maxLength\": 2000,\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A human-readable description\
  \ of the feature flag and its purpose\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the feature flag was created\"\n    },\n    \"initial_value\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The initial value assigned to the feature when it was created\"\n    },\n    \"default_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the feature flag is enabled by default in new environments\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"STANDARD\", \"MULTIVARIATE\"],\n      \"description\": \"The type of feature flag. STANDARD for simple on/off flags with an optional value, MULTIVARIATE for flags with multiple weighted value variations\"\n    },\n    \"project\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project this feature flag belongs to\"\n    },\n    \"is_archived\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether the feature flag is archived and hidden from the dashboard by default\"\n    },\n    \"owners\": {\n      \"type\": \"array\",\n      \"description\": \"The users who are designated as owners of this feature flag\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FeatureOwner\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of tags associated with this feature flag for organization\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"multivariate_options\": {\n      \"type\": \"array\",\n      \"description\": \"The multivariate value options available for this feature flag when the type is MULTIVARIATE\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MultivariateOption\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"FeatureOwner\": {\n      \"type\": \"object\",\n      \"description\": \"A user designated as an owner of a feature flag\",\n      \"properties\":\
  \ {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for the user\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the user\"\n        }\n      }\n    },\n    \"MultivariateOption\": {\n      \"type\": \"object\",\n      \"description\": \"A value variation for a multivariate feature flag with a percentage allocation\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for this multivariate option\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the option value\"\n        },\n        \"string_value\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The string value of this option\"\n        },\n        \"integer_value\": {\n          \"type\": [\"integer\"\
  , \"null\"],\n          \"description\": \"The integer value of this option\"\n        },\n        \"boolean_value\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"The boolean value of this option\"\n        },\n        \"default_percentage_allocation\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"The default percentage of users who will receive this value variation\"\n        }\n      }\n    },\n    \"FeatureState\": {\n      \"type\": \"object\",\n      \"description\": \"The state of a feature flag within a specific environment, including its enabled status and current value\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for this feature state\"\n        },\n        \"feature\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the feature flag\"\n        },\n     \
  \   \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the feature flag is currently enabled in this environment\"\n        },\n        \"feature_state_value\": {\n          \"description\": \"The current value of the feature flag in this environment\",\n          \"type\": [\"string\", \"integer\", \"boolean\", \"null\"]\n        },\n        \"environment\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the environment\"\n        },\n        \"identity\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The identity ID if this is an identity-specific override\"\n        },\n        \"feature_segment\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The feature segment ID if this is a segment override\"\n        }\n      }\n    },\n    \"Segment\": {\n      \"type\": \"object\",\n      \"description\": \"A segment defining a group of users based on trait-based rules\
  \ for targeted flag delivery\",\n      \"required\": [\"name\", \"rules\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for this segment\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the segment\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A description of the segment and its targeting criteria\"\n        },\n        \"project\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the project this segment belongs to\"\n        },\n        \"rules\": {\n          \"type\": \"array\",\n          \"description\": \"The rules that define membership in this segment\",\n          \"items\": {\n            \"$ref\": \"#/$defs/SegmentRule\"\n          }\n        }\n      }\n    },\n    \"SegmentRule\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A rule within a segment combining conditions with logical operators\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"ALL\", \"ANY\", \"NONE\"],\n          \"description\": \"The logical operator for combining conditions. ALL requires all conditions to match, ANY requires at least one, NONE requires none to match\"\n        },\n        \"rules\": {\n          \"type\": \"array\",\n          \"description\": \"Nested sub-rules for complex targeting logic\",\n          \"items\": {\n            \"$ref\": \"#/$defs/SegmentRule\"\n          }\n        },\n        \"conditions\": {\n          \"type\": \"array\",\n          \"description\": \"The trait-based conditions that make up this rule\",\n          \"items\": {\n            \"$ref\": \"#/$defs/SegmentCondition\"\n          }\n        }\n      }\n    },\n    \"SegmentCondition\": {\n      \"type\": \"object\",\n      \"description\": \"A condition evaluating a user trait against\
  \ a value using a comparison operator\",\n      \"properties\": {\n        \"operator\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"EQUAL\",\n            \"NOT_EQUAL\",\n            \"GREATER_THAN\",\n            \"GREATER_THAN_INCLUSIVE\",\n            \"LESS_THAN\",\n            \"LESS_THAN_INCLUSIVE\",\n            \"CONTAINS\",\n            \"NOT_CONTAINS\",\n            \"REGEX\",\n            \"PERCENTAGE_SPLIT\",\n            \"IS_SET\",\n            \"IS_NOT_SET\",\n            \"IN\"\n          ],\n          \"description\": \"The comparison operator to use when evaluating the trait\"\n        },\n        \"property_\": {\n          \"type\": \"string\",\n          \"description\": \"The trait key to evaluate against\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value to compare the trait against\"\n        }\n      }\n    },\n    \"Identity\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A user identity within an environment with associated traits\",\n      \"required\": [\"identifier\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for this identity\"\n        },\n        \"identifier\": {\n          \"type\": \"string\",\n          \"description\": \"The user-provided identifier for this identity, typically a user ID or email\"\n        },\n        \"environment\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the environment this identity belongs to\"\n        },\n        \"traits\": {\n          \"type\": \"array\",\n          \"description\": \"The traits associated with this identity\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Trait\"\n          }\n        }\n      }\n    },\n    \"Trait\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair associated with an identity used for segment evaluation and personalized\
  \ flag delivery\",\n      \"required\": [\"trait_key\", \"trait_value\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for this trait\"\n        },\n        \"trait_key\": {\n          \"type\": \"string\",\n          \"description\": \"The key name of the trait\"\n        },\n        \"trait_value\": {\n          \"description\": \"The value of the trait, which can be a string, integer, float, or boolean\",\n          \"type\": [\"string\", \"integer\", \"number\", \"boolean\"]\n        },\n        \"transient\": {\n          \"type\": \"boolean\",\n          \"description\": \"When true, this trait is used for evaluation only and is not persisted\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/json-schema/flagsmith-feature-flag-schema.json
tags: []
title: Flagsmith Feature Flag
---
