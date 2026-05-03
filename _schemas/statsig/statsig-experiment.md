---
description: An A/B test experiment configuration with defined groups, parameter values, allocation percentages, and analysis settings. Experiments enable controlled testing of product changes by splitting users into groups and measuring metric impacts.
layout: schema
name: Statsig Experiment
properties_list:
- description: The unique identifier of the experiment.
  name: id
  type: string
- description: The name of the experiment, used as the key for SDK evaluation.
  name: name
  type: string
- description: A human-readable description of the experiment and what it tests.
  name: description
  type: string
- description: The hypothesis being tested, describing the expected outcome of the experiment.
  name: hypothesis
  type: string
- description: The current lifecycle status of the experiment.
  name: status
  type: string
- description: The experiment groups defining parameter values for each user segment.
  name: groups
  type: array
- description: The percentage of eligible users allocated to the experiment.
  name: allocation
  type: number
- description: The layer this experiment belongs to, enabling parameter sharing and mutual exclusivity with other experiments.
  name: layerID
  type: string
- description: The feature gate used to filter which users are eligible for the experiment.
  name: targetingGateID
  type: string
- description: The default parameter values returned when a user is not allocated to the experiment.
  name: defaultValues
  type: object
- description: The primary metrics used to evaluate the experiment hypothesis.
  name: primaryMetrics
  type: array
- description: Secondary metrics monitored during the experiment for guardrail and exploratory analysis.
  name: secondaryMetrics
  type: array
- description: Tags for organizing and categorizing the experiment.
  name: tags
  type: array
- description: Target applications this experiment is scoped to.
  name: targetApps
  type: array
- description: Timestamp in milliseconds since epoch when the experiment was started.
  name: startedTime
  type: integer
- description: Timestamp in milliseconds since epoch when the experiment was created.
  name: createdTime
  type: integer
- description: Timestamp in milliseconds since epoch when the experiment was last modified.
  name: lastModifiedTime
  type: integer
provider_name: statsig
provider_slug: statsig
schema_file: json-schema/statsig-experiment-schema.json
slug: statsig-experiment
source_filename: statsig-experiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.statsig.com/schemas/statsig/experiment.json\",\n  \"title\": \"Statsig Experiment\",\n  \"description\": \"An A/B test experiment configuration with defined groups, parameter values, allocation percentages, and analysis settings. Experiments enable controlled testing of product changes by splitting users into groups and measuring metric impacts.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the experiment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the experiment, used as the key for SDK evaluation.\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the experiment and what it tests.\"\
  ,\n      \"maxLength\": 4096\n    },\n    \"hypothesis\": {\n      \"type\": \"string\",\n      \"description\": \"The hypothesis being tested, describing the expected outcome of the experiment.\",\n      \"maxLength\": 4096\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current lifecycle status of the experiment.\",\n      \"enum\": [\"setup\", \"active\", \"decision_made\", \"abandoned\"]\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"The experiment groups defining parameter values for each user segment.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ExperimentGroup\"\n      },\n      \"minItems\": 2\n    },\n    \"allocation\": {\n      \"type\": \"number\",\n      \"description\": \"The percentage of eligible users allocated to the experiment.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"default\": 100\n    },\n    \"layerID\": {\n      \"type\": \"string\",\n      \"description\": \"The layer\
  \ this experiment belongs to, enabling parameter sharing and mutual exclusivity with other experiments.\"\n    },\n    \"targetingGateID\": {\n      \"type\": \"string\",\n      \"description\": \"The feature gate used to filter which users are eligible for the experiment.\"\n    },\n    \"defaultValues\": {\n      \"type\": \"object\",\n      \"description\": \"The default parameter values returned when a user is not allocated to the experiment.\",\n      \"additionalProperties\": true\n    },\n    \"primaryMetrics\": {\n      \"type\": \"array\",\n      \"description\": \"The primary metrics used to evaluate the experiment hypothesis.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetricReference\"\n      }\n    },\n    \"secondaryMetrics\": {\n      \"type\": \"array\",\n      \"description\": \"Secondary metrics monitored during the experiment for guardrail and exploratory analysis.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetricReference\"\n      }\n    },\n    \"\
  tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags for organizing and categorizing the experiment.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"targetApps\": {\n      \"type\": \"array\",\n      \"description\": \"Target applications this experiment is scoped to.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"startedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp in milliseconds since epoch when the experiment was started.\"\n    },\n    \"createdTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp in milliseconds since epoch when the experiment was created.\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp in milliseconds since epoch when the experiment was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"ExperimentGroup\": {\n      \"type\": \"object\",\n      \"description\": \"An experiment group\
  \ that defines parameter values for a segment of allocated users.\",\n      \"required\": [\"name\", \"size\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the group (e.g., control, test, variant_a).\",\n          \"minLength\": 1\n        },\n        \"size\": {\n          \"type\": \"number\",\n          \"description\": \"The percentage of allocated users assigned to this group. All group sizes must sum to 100.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"parameterValues\": {\n          \"type\": \"object\",\n          \"description\": \"The parameter key-value pairs for users in this group.\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"MetricReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a metric definition used in experiment analysis.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n  \
  \      \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the metric.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The metric type (e.g., event_count, ratio, funnel, mean).\"\n        },\n        \"direction\": {\n          \"type\": \"string\",\n          \"description\": \"The expected direction of change for this metric.\",\n          \"enum\": [\"increase\", \"decrease\"]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/json-schema/statsig-experiment-schema.json
tags: []
title: Statsig Experiment
---
