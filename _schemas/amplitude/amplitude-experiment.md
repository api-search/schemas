---
description: Schema for an Amplitude experiment or feature flag configuration including variants, targeting segments, and deployment settings.
layout: schema
name: Amplitude Experiment
properties_list:
- description: The unique identifier for the experiment or flag.
  name: id
  type: string
- description: The project ID the experiment belongs to.
  name: projectId
  type: string
- description: The unique key used to reference the experiment or flag in code.
  name: key
  type: string
- description: The display name of the experiment or flag.
  name: name
  type: string
- description: A description of the experiment's purpose and hypothesis.
  name: description
  type: string
- description: The type of configuration.
  name: type
  type: string
- description: Whether the experiment or flag is currently enabled.
  name: enabled
  type: boolean
- description: The evaluation mode determining where variants are computed.
  name: evaluationMode
  type: string
- description: The lifecycle state of the experiment or flag.
  name: state
  type: string
- description: The user property used for deterministic bucketing.
  name: bucketingKey
  type: string
- description: The salt used with the bucketing key for hash computation.
  name: bucketingSalt
  type: string
- description: Array of variant configurations for the experiment.
  name: variants
  type: array
- description: Array of targeting segments that control which users see which variants.
  name: segments
  type: array
- description: Array of deployment IDs where this experiment is active.
  name: deployments
  type: array
- description: The variant key that was rolled out after the experiment concluded.
  name: rolledOutVariant
  type: string
- description: The date and time the experiment started.
  name: startDate
  type: string
- description: The date and time the experiment ended.
  name: endDate
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/amplitude-experiment-schema.json
slug: amplitude-experiment
source_filename: amplitude-experiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://amplitude.com/schemas/amplitude/experiment.json\",\n  \"title\": \"Amplitude Experiment\",\n  \"description\": \"Schema for an Amplitude experiment or feature flag configuration including variants, targeting segments, and deployment settings.\",\n  \"type\": \"object\",\n  \"required\": [\"key\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the experiment or flag.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID the experiment belongs to.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key used to reference the experiment or flag in code.\",\n      \"minLength\": 1,\n      \"pattern\": \"^[a-z0-9_-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the experiment or\
  \ flag.\",\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the experiment's purpose and hypothesis.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of configuration.\",\n      \"enum\": [\"experiment\", \"flag\", \"release\"]\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the experiment or flag is currently enabled.\"\n    },\n    \"evaluationMode\": {\n      \"type\": \"string\",\n      \"description\": \"The evaluation mode determining where variants are computed.\",\n      \"enum\": [\"local\", \"remote\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state of the experiment or flag.\",\n      \"enum\": [\"draft\", \"running\", \"stopped\", \"active\", \"archived\"]\n    },\n    \"bucketingKey\": {\n      \"type\": \"string\",\n      \"description\": \"The user property\
  \ used for deterministic bucketing.\"\n    },\n    \"bucketingSalt\": {\n      \"type\": \"string\",\n      \"description\": \"The salt used with the bucketing key for hash computation.\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"Array of variant configurations for the experiment.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Variant\"\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of targeting segments that control which users see which variants.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Segment\"\n      }\n    },\n    \"deployments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of deployment IDs where this experiment is active.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"rolledOutVariant\": {\n      \"type\": \"string\",\n      \"description\": \"The variant key that was rolled out after the experiment concluded.\"\n    },\n  \
  \  \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the experiment started.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the experiment ended.\"\n    }\n  },\n  \"$defs\": {\n    \"Variant\": {\n      \"type\": \"object\",\n      \"description\": \"A variant in an experiment or feature flag.\",\n      \"required\": [\"key\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The unique key identifying this variant.\",\n          \"minLength\": 1\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the variant.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of what this variant does.\"\n        },\n        \"payload\": {\n          \"\
  description\": \"An optional JSON payload associated with the variant for client-side configuration.\"\n        },\n        \"rolloutWeight\": {\n          \"type\": \"integer\",\n          \"description\": \"The traffic allocation percentage for this variant.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    },\n    \"Segment\": {\n      \"type\": \"object\",\n      \"description\": \"A targeting segment that defines which users receive a specific variant.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the segment.\"\n        },\n        \"conditions\": {\n          \"type\": \"array\",\n          \"description\": \"Array of targeting conditions that must all be true for the segment to match.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Condition\"\n          }\n        },\n        \"variant\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The variant key to assign when this segment matches.\"\n        },\n        \"percentage\": {\n          \"type\": \"integer\",\n          \"description\": \"The percentage of matching users to include.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    },\n    \"Condition\": {\n      \"type\": \"object\",\n      \"description\": \"A single targeting condition used in segment evaluation.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of targeting condition.\",\n          \"enum\": [\"user_property\", \"cohort\", \"device_id\", \"user_id\"]\n        },\n        \"prop\": {\n          \"type\": \"string\",\n          \"description\": \"The property name to evaluate.\"\n        },\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator.\",\n          \"enum\": [\"is\", \"is_not\", \"contains\", \"does_not_contain\", \"greater_than\"\
  , \"less_than\", \"set\", \"not_set\", \"glob_match\", \"glob_does_not_match\"]\n        },\n        \"values\": {\n          \"type\": \"array\",\n          \"description\": \"The values to compare against.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/amplitude-experiment-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Amplitude Experiment
---
