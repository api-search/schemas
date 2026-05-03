---
description: Represents a Workato recipe — an automated workflow connecting applications and services. Recipes consist of a trigger and one or more actions that run when the trigger fires.
layout: schema
name: Workato Recipe
properties_list:
- description: Unique integer identifier of the recipe within the workspace.
  name: id
  type: integer
- description: Display name of the recipe shown in the Workato UI.
  name: name
  type: string
- description: Human-readable explanation of what the recipe does and when it runs.
  name: description
  type: string
- description: ID of the workspace folder that contains this recipe.
  name: folder_id
  type: integer
- description: Whether the recipe is currently active and processing trigger events.
  name: running
  type: boolean
- description: Name of the connector used for the recipe's trigger event.
  name: trigger_application
  type: string
- description: List of connector names used in the recipe's action steps.
  name: action_applications
  type: array
- description: JSON-encoded recipe definition containing trigger and action configurations.
  name: code
  type: string
- description: JSON-encoded recipe configuration for connection mappings and settings.
  name: config
  type: string
- description: Reason the recipe was last stopped (e.g., error, manual stop).
  name: stop_cause
  type: string
- description: ISO 8601 timestamp when the recipe was created.
  name: created_at
  type: string
- description: ISO 8601 timestamp when the recipe was last modified.
  name: updated_at
  type: string
- description: ISO 8601 timestamp when the recipe was last stopped, if applicable.
  name: stopped_at
  type: string
- description: ISO 8601 timestamp of the most recent recipe job execution.
  name: last_run_at
  type: string
- description: Total number of successfully completed jobs for this recipe.
  name: job_succeeded_count
  type: integer
- description: Total number of failed jobs for this recipe.
  name: job_failed_count
  type: integer
- description: Current version number of the recipe.
  name: version_no
  type: integer
provider_name: Workato
provider_slug: workato
schema_file: json-schema/workato-recipe-schema.json
slug: workato-recipe
source_filename: workato-recipe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.workato.com/schemas/recipe.json\",\n  \"title\": \"Workato Recipe\",\n  \"description\": \"Represents a Workato recipe — an automated workflow connecting applications and services. Recipes consist of a trigger and one or more actions that run when the trigger fires.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique integer identifier of the recipe within the workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the recipe shown in the Workato UI.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable explanation of what the recipe does and when it runs.\"\n    },\n    \"folder_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the workspace\
  \ folder that contains this recipe.\"\n    },\n    \"running\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the recipe is currently active and processing trigger events.\"\n    },\n    \"trigger_application\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the connector used for the recipe's trigger event.\"\n    },\n    \"action_applications\": {\n      \"type\": \"array\",\n      \"description\": \"List of connector names used in the recipe's action steps.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Connector name.\"\n      }\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"JSON-encoded recipe definition containing trigger and action configurations.\"\n    },\n    \"config\": {\n      \"type\": \"string\",\n      \"description\": \"JSON-encoded recipe configuration for connection mappings and settings.\"\n    },\n    \"stop_cause\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Reason the recipe was last stopped (e.g., error, manual stop).\",\n      \"enum\": [\"error\", \"manual\", \"test_mode_limit\", \"task_limit\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the recipe was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the recipe was last modified.\"\n    },\n    \"stopped_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the recipe was last stopped, if applicable.\"\n    },\n    \"last_run_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the most recent recipe job execution.\"\n    },\n    \"job_succeeded_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total number of\
  \ successfully completed jobs for this recipe.\"\n    },\n    \"job_failed_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total number of failed jobs for this recipe.\"\n    },\n    \"version_no\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Current version number of the recipe.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"$defs\": {\n    \"RecipeVersion\": {\n      \"type\": \"object\",\n      \"title\": \"Recipe Version\",\n      \"description\": \"A specific version snapshot of a recipe, created each time the recipe is saved.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of this version record.\"\n        },\n        \"version_no\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Sequential version number, incrementing with each save.\"\n        },\n        \"comment\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Optional description of what changed in this version.\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"JSON-encoded recipe definition at this version.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this version was saved.\"\n        }\n      },\n      \"required\": [\"id\", \"version_no\"]\n    },\n    \"RecipeJob\": {\n      \"type\": \"object\",\n      \"title\": \"Recipe Job\",\n      \"description\": \"A single execution instance of a recipe triggered by an event.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the job.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the job execution.\",\n         \
  \ \"enum\": [\"succeeded\", \"failed\", \"pending\", \"running\"]\n        },\n        \"started_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the job started executing.\"\n        },\n        \"completed_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the job finished executing.\"\n        },\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"Error message if the job failed.\"\n        }\n      },\n      \"required\": [\"id\", \"status\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/json-schema/workato-recipe-schema.json
tags:
- Agentic
- API Management
- Automation
- B2B
- Embedded iPaaS
- Enterprise
- Integration
- iPaaS
- Orchestration
- Workflow
title: Workato Recipe
---
