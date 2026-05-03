---
description: Schema representing an A/B test experiment in Optimizely, including variations, metrics, audience targeting, and traffic allocation configuration.
layout: schema
name: Optimizely Experiment
properties_list:
- description: Unique identifier for the experiment
  name: id
  type: integer
- description: The project this experiment belongs to
  name: project_id
  type: integer
- description: Human-readable name of the experiment
  name: name
  type: string
- description: Description of the experiment purpose and hypothesis
  name: description
  type: string
- description: Current lifecycle status of the experiment
  name: status
  type: string
- description: Type of experiment design
  name: type
  type: string
- description: Percentage of traffic held back from the experiment, expressed in basis points (0-10000)
  name: holdback
  type: integer
- description: List of variations presented to visitors in the experiment
  name: variations
  type: array
- description: List of metrics used to measure experiment results
  name: metrics
  type: array
- description: JSON-encoded audience targeting conditions that determine which visitors see the experiment
  name: audience_conditions
  type: string
- description: List of page IDs where the experiment runs
  name: page_ids
  type: array
- description: Timestamp when the experiment was created
  name: created
  type: string
- description: Timestamp when the experiment was last modified
  name: last_modified
  type: string
provider_name: Optimizely
provider_slug: optimizely
schema_file: json-schema/optimizely-experiment-schema.json
slug: optimizely-experiment
source_filename: optimizely-experiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.optimizely.com/schemas/optimizely/experiment.json\",\n  \"title\": \"Optimizely Experiment\",\n  \"description\": \"Schema representing an A/B test experiment in Optimizely, including variations, metrics, audience targeting, and traffic allocation configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"project_id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the experiment\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The project this experiment belongs to\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the experiment\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the experiment purpose and\
  \ hypothesis\",\n      \"maxLength\": 2000\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the experiment\",\n      \"enum\": [\"active\", \"paused\", \"not_started\", \"archived\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of experiment design\",\n      \"enum\": [\"a/b\", \"multiarmed_bandit\", \"multivariate\"]\n    },\n    \"holdback\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of traffic held back from the experiment, expressed in basis points (0-10000)\",\n      \"minimum\": 0,\n      \"maximum\": 10000\n    },\n    \"variations\": {\n      \"type\": \"array\",\n      \"description\": \"List of variations presented to visitors in the experiment\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Variation\"\n      },\n      \"minItems\": 2\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"List of metrics used to measure\
  \ experiment results\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Metric\"\n      }\n    },\n    \"audience_conditions\": {\n      \"type\": \"string\",\n      \"description\": \"JSON-encoded audience targeting conditions that determine which visitors see the experiment\"\n    },\n    \"page_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of page IDs where the experiment runs\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the experiment was created\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the experiment was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Variation\": {\n      \"type\": \"object\",\n      \"description\": \"A variation within an experiment that represents a distinct experience shown to visitors\"\
  ,\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"variation_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier for the variation\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Unique key for the variation within the experiment\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the variation\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"weight\": {\n          \"type\": \"integer\",\n          \"description\": \"Traffic allocation weight in basis points (0-10000)\",\n          \"minimum\": 0,\n          \"maximum\": 10000\n        },\n        \"actions\": {\n          \"type\": \"array\",\n          \"description\": \"Changes applied when this variation is shown\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Action\"\n          }\n        }\n      }\n    },\n\
  \    \"Action\": {\n      \"type\": \"object\",\n      \"description\": \"A set of changes applied to a page in a variation\",\n      \"properties\": {\n        \"page_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The page this action applies to\"\n        },\n        \"changes\": {\n          \"type\": \"array\",\n          \"description\": \"Individual changes applied on the page\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Type of change (e.g., custom_code, attribute, insert_html)\"\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"The change value or code\"\n              },\n              \"selector\": {\n                \"type\": \"string\",\n                \"description\": \"CSS selector targeting the element to modify\"\n            \
  \  }\n            }\n          }\n        }\n      }\n    },\n    \"Metric\": {\n      \"type\": \"object\",\n      \"description\": \"A metric definition for measuring experiment outcomes\",\n      \"required\": [\"event_id\", \"aggregator\"],\n      \"properties\": {\n        \"event_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The event ID this metric tracks\"\n        },\n        \"aggregator\": {\n          \"type\": \"string\",\n          \"description\": \"How to aggregate the metric values\",\n          \"enum\": [\"unique\", \"count\", \"sum\"]\n        },\n        \"field\": {\n          \"type\": \"string\",\n          \"description\": \"The field to aggregate on for sum aggregation\"\n        },\n        \"scope\": {\n          \"type\": \"string\",\n          \"description\": \"The scope at which to measure the metric\",\n          \"enum\": [\"visitor\", \"session\", \"event\"]\n        },\n        \"winning_direction\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Which direction indicates improvement\",\n          \"enum\": [\"increasing\", \"decreasing\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/json-schema/optimizely-experiment-schema.json
tags:
- A/B Testing
- Content Management
- Customer Data
- E-Commerce
- Experimentation
- Feature Flags
- Marketing
title: Optimizely Experiment
---
