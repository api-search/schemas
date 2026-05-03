---
description: Schema for the redocly.yaml configuration file used by the Redocly CLI, Realm, and other Redocly tools.
layout: schema
name: Redocly Configuration
properties_list:
- description: Map of named API definitions. Each key is an API name, each value is an API configuration.
  name: apis
  type: object
- description: 'Base ruleset(s) to extend. Built-in values: spec, recommended, recommended-strict, minimal.'
  name: extends
  type: object
- description: Rule configuration map. Keys are rule names, values are off/warn/error or rule config objects.
  name: rules
  type: object
- description: Theming configuration for Realm/Revel portals.
  name: theme
  type: object
- description: List of Redocly CLI plugin paths.
  name: plugins
  type: array
- description: Decorator configuration for transforming OpenAPI during bundling.
  name: decorators
  type: object
- description: Preprocessor configuration applied before rules.
  name: preprocessors
  type: object
provider_name: Redocly
provider_slug: redocly
schema_file: json-schema/redocly-config-schema.json
slug: redocly-config
source_filename: redocly-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redocly.com/schemas/redocly.yaml\",\n  \"title\": \"Redocly Configuration\",\n  \"description\": \"Schema for the redocly.yaml configuration file used by the Redocly CLI, Realm, and other Redocly tools.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apis\": {\n      \"type\": \"object\",\n      \"description\": \"Map of named API definitions. Each key is an API name, each value is an API configuration.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/ApiDefinition\"\n      }\n    },\n    \"extends\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Base ruleset(s) to extend. Built-in values: spec, recommended, recommended-strict, minimal.\"\n    },\n    \"rules\": {\n      \"type\": \"object\",\n      \"description\": \"Rule configuration map. Keys\
  \ are rule names, values are off/warn/error or rule config objects.\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          { \"type\": \"string\", \"enum\": [\"off\", \"warn\", \"error\"] },\n          {\n            \"type\": \"object\",\n            \"properties\": {\n              \"severity\": { \"type\": \"string\", \"enum\": [\"off\", \"warn\", \"error\"] }\n            }\n          }\n        ]\n      }\n    },\n    \"theme\": {\n      \"type\": \"object\",\n      \"description\": \"Theming configuration for Realm/Revel portals.\",\n      \"properties\": {\n        \"openapi\": {\n          \"type\": \"object\",\n          \"description\": \"OpenAPI reference documentation theming.\"\n        },\n        \"logo\": {\n          \"type\": \"object\",\n          \"description\": \"Logo configuration.\"\n        }\n      }\n    },\n    \"plugins\": {\n      \"type\": \"array\",\n      \"description\": \"List of Redocly CLI plugin paths.\",\n      \"items\": { \"type\"\
  : \"string\" }\n    },\n    \"decorators\": {\n      \"type\": \"object\",\n      \"description\": \"Decorator configuration for transforming OpenAPI during bundling.\"\n    },\n    \"preprocessors\": {\n      \"type\": \"object\",\n      \"description\": \"Preprocessor configuration applied before rules.\"\n    }\n  },\n  \"$defs\": {\n    \"ApiDefinition\": {\n      \"type\": \"object\",\n      \"required\": [\"root\"],\n      \"properties\": {\n        \"root\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the root OpenAPI definition file.\"\n        },\n        \"extends\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ],\n          \"description\": \"Override base ruleset for this specific API.\"\n        },\n        \"rules\": {\n          \"type\": \"object\",\n          \"description\": \"Per-API rule overrides.\"\n        },\n        \"labels\": {\n\
  \          \"type\": \"array\",\n          \"description\": \"Labels for organizing APIs in Realm catalog.\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/json-schema/redocly-config-schema.json
tags:
- API Catalog
- API Documentation
- Developer Portal
- Governance
- Linting
- OpenAPI
title: Redocly Configuration
---
