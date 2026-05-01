---
description: Top-level configuration for a Databricks Asset Bundle (databricks.yml).
layout: schema
name: Databricks Asset Bundle
properties_list:
- description: Core bundle metadata.
  name: bundle
  type: object
- description: Glob patterns of additional configuration files to include.
  name: include
  type: array
- description: Workspace connection and path settings.
  name: workspace
  type: object
- description: Custom variable declarations.
  name: variables
  type: object
- description: Artifacts (such as Python wheels) built during deployment.
  name: artifacts
  type: object
- description: ''
  name: resources
  type: object
- description: Environment-specific overrides (dev, staging, prod).
  name: targets
  type: object
- description: ''
  name: permissions
  type: array
- description: Deployment behavior customization across resources.
  name: presets
  type: object
- description: Identity used to run jobs and pipelines.
  name: run_as
  type: object
- description: Named commands executable via 'databricks bundle run'.
  name: scripts
  type: object
- description: File inclusion and exclusion patterns for deployment sync.
  name: sync
  type: object
- description: Beta feature flags.
  name: experimental
  type: object
- description: Python loader and mutator configuration.
  name: python
  type: object
provider_name: Databricks Asset Bundles
provider_slug: databricks-asset-bundles
schema_file: json-schema/bundle.json
slug: bundle
source_filename: bundle.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/databricks-asset-bundles/main/json-schema/bundle.json\",\n  \"title\": \"Databricks Asset Bundle\",\n  \"description\": \"Top-level configuration for a Databricks Asset Bundle (databricks.yml).\",\n  \"type\": \"object\",\n  \"required\": [\"bundle\"],\n  \"additionalProperties\": false,\n  \"properties\": {\n    \"bundle\": {\n      \"type\": \"object\",\n      \"description\": \"Core bundle metadata.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\"type\": \"string\", \"description\": \"Programmatic bundle name.\"},\n        \"uuid\": {\"type\": \"string\", \"description\": \"Optional unique bundle identifier.\"},\n        \"databricks_cli_version\": {\"type\": \"string\", \"description\": \"Semver constraint for the Databricks CLI.\"},\n        \"git\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"branch\": {\"type\": \"string\"},\n            \"origin_url\": {\"type\": \"string\", \"format\": \"uri\"}\n          }\n        },\n        \"deployment\": {\"type\": \"object\"}\n      }\n    },\n    \"include\": {\n      \"type\": \"array\",\n      \"description\": \"Glob patterns of additional configuration files to include.\",\n      \"items\": {\"type\": \"string\"}\n    },\n    \"workspace\": {\n      \"type\": \"object\",\n      \"description\": \"Workspace connection and path settings.\",\n      \"properties\": {\n        \"host\": {\"type\": \"string\", \"format\": \"uri\"},\n        \"profile\": {\"type\": \"string\"},\n        \"auth_type\": {\"type\": \"string\"},\n        \"root_path\": {\"type\": \"string\", \"pattern\": \"^/Workspace|^/Volumes\"},\n        \"file_path\": {\"type\": \"string\"},\n        \"artifact_path\": {\"type\": \"string\"},\n        \"state_path\": {\"type\": \"string\"}\n      }\n    },\n    \"variables\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Custom variable declarations.\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\"type\": \"string\"},\n          {\n            \"type\": \"object\",\n            \"properties\": {\n              \"description\": {\"type\": \"string\"},\n              \"default\": {},\n              \"type\": {\"type\": \"string\"},\n              \"lookup\": {\"type\": \"object\"}\n            }\n          }\n        ]\n      }\n    },\n    \"artifacts\": {\n      \"type\": \"object\",\n      \"description\": \"Artifacts (such as Python wheels) built during deployment.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\"type\": \"string\", \"enum\": [\"whl\", \"jar\"]},\n          \"build\": {\"type\": \"string\"},\n          \"executable\": {\"type\": \"string\"},\n          \"path\": {\"type\": \"string\"},\n          \"files\": {\"type\": \"array\", \"items\": {\"type\": \"\
  object\"}}\n        }\n      }\n    },\n    \"resources\": {\n      \"$ref\": \"#/$defs/resources\"\n    },\n    \"targets\": {\n      \"type\": \"object\",\n      \"description\": \"Environment-specific overrides (dev, staging, prod).\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"default\": {\"type\": \"boolean\"},\n          \"mode\": {\"type\": \"string\", \"enum\": [\"development\", \"production\"]},\n          \"workspace\": {\"$ref\": \"#/properties/workspace\"},\n          \"variables\": {\"$ref\": \"#/properties/variables\"},\n          \"resources\": {\"$ref\": \"#/$defs/resources\"},\n          \"presets\": {\"type\": \"object\"},\n          \"run_as\": {\"type\": \"object\"},\n          \"permissions\": {\"type\": \"array\", \"items\": {\"$ref\": \"#/$defs/permission\"}},\n          \"sync\": {\"type\": \"object\"}\n        }\n      }\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"items\": {\"\
  $ref\": \"#/$defs/permission\"}\n    },\n    \"presets\": {\n      \"type\": \"object\",\n      \"description\": \"Deployment behavior customization across resources.\"\n    },\n    \"run_as\": {\n      \"type\": \"object\",\n      \"description\": \"Identity used to run jobs and pipelines.\",\n      \"properties\": {\n        \"user_name\": {\"type\": \"string\"},\n        \"service_principal_name\": {\"type\": \"string\"}\n      }\n    },\n    \"scripts\": {\n      \"type\": \"object\",\n      \"description\": \"Named commands executable via 'databricks bundle run'.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"content\": {\"type\": \"string\"}\n        }\n      }\n    },\n    \"sync\": {\n      \"type\": \"object\",\n      \"description\": \"File inclusion and exclusion patterns for deployment sync.\",\n      \"properties\": {\n        \"include\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}},\n        \"exclude\"\
  : {\"type\": \"array\", \"items\": {\"type\": \"string\"}},\n        \"paths\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}}\n      }\n    },\n    \"experimental\": {\n      \"type\": \"object\",\n      \"description\": \"Beta feature flags.\"\n    },\n    \"python\": {\n      \"type\": \"object\",\n      \"description\": \"Python loader and mutator configuration.\"\n    }\n  },\n  \"$defs\": {\n    \"permission\": {\n      \"type\": \"object\",\n      \"required\": [\"level\"],\n      \"properties\": {\n        \"level\": {\"type\": \"string\", \"enum\": [\"CAN_VIEW\", \"CAN_RUN\", \"CAN_MANAGE\", \"IS_OWNER\"]},\n        \"user_name\": {\"type\": \"string\"},\n        \"service_principal_name\": {\"type\": \"string\"},\n        \"group_name\": {\"type\": \"string\"}\n      }\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"description\": \"Databricks resources to deploy as part of the bundle.\",\n      \"properties\": {\n        \"alerts\": {\"type\": \"\
  object\"},\n        \"apps\": {\"type\": \"object\"},\n        \"catalogs\": {\"type\": \"object\"},\n        \"clusters\": {\"type\": \"object\"},\n        \"dashboards\": {\"type\": \"object\"},\n        \"database_catalogs\": {\"type\": \"object\"},\n        \"database_instances\": {\"type\": \"object\"},\n        \"experiments\": {\"type\": \"object\"},\n        \"external_locations\": {\"type\": \"object\"},\n        \"jobs\": {\"type\": \"object\"},\n        \"model_serving_endpoints\": {\"type\": \"object\"},\n        \"models\": {\"type\": \"object\"},\n        \"pipelines\": {\"type\": \"object\"},\n        \"postgres_branches\": {\"type\": \"object\"},\n        \"postgres_endpoints\": {\"type\": \"object\"},\n        \"postgres_projects\": {\"type\": \"object\"},\n        \"quality_monitors\": {\"type\": \"object\"},\n        \"registered_models\": {\"type\": \"object\"},\n        \"schemas\": {\"type\": \"object\"},\n        \"secret_scopes\": {\"type\": \"object\"},\n     \
  \   \"sql_warehouses\": {\"type\": \"object\"},\n        \"synced_database_tables\": {\"type\": \"object\"},\n        \"volumes\": {\"type\": \"object\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks-asset-bundles/refs/heads/main/json-schema/bundle.json
tags:
- CI/CD
- Data Engineering
- Databricks
- Deployment
- Infrastructure as Code
- Jobs
- Machine Learning
- MLOps
- Pipelines
- Workflows
title: Databricks Asset Bundle
---
