---
description: An event object used for logging exposure events, custom events, and webhook payloads in the Statsig analytics pipeline. Events power experiment analysis, product analytics, and metric computations.
layout: schema
name: Statsig Event
properties_list:
- description: 'The name of the event. Exposure events use the format statsig::gate_exposure, statsig::config_exposure, or statsig::experiment_exposure. Config change events use statsig::config_change. Custom events '
  name: eventName
  type: string
- description: ''
  name: user
  type: object
- description: Timestamp of the event in milliseconds since epoch.
  name: time
  type: integer
- description: An optional value associated with the event, such as a revenue amount, duration, or string label.
  name: value
  type: object
- description: Optional metadata key-value pairs providing additional context for the event.
  name: metadata
  type: object
- description: ''
  name: statsigMetadata
  type: object
- description: A unique identifier for this event instance, combining timestamp and random components.
  name: timeUUID
  type: string
provider_name: statsig
provider_slug: statsig
schema_file: json-schema/statsig-event-schema.json
slug: statsig-event
source_filename: statsig-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.statsig.com/schemas/statsig/event.json\",\n  \"title\": \"Statsig Event\",\n  \"description\": \"An event object used for logging exposure events, custom events, and webhook payloads in the Statsig analytics pipeline. Events power experiment analysis, product analytics, and metric computations.\",\n  \"type\": \"object\",\n  \"required\": [\"eventName\", \"user\", \"time\"],\n  \"properties\": {\n    \"eventName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event. Exposure events use the format statsig::gate_exposure, statsig::config_exposure, or statsig::experiment_exposure. Config change events use statsig::config_change. Custom events use application-defined names.\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/StatsigUser\"\n    },\n    \"time\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Timestamp of the event in milliseconds since epoch.\",\n      \"format\": \"int64\"\n    },\n    \"value\": {\n      \"description\": \"An optional value associated with the event, such as a revenue amount, duration, or string label.\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"number\" }\n      ]\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Optional metadata key-value pairs providing additional context for the event.\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"gate\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the gate, for gate exposure events.\"\n        },\n        \"config\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the config or experiment, for config or experiment exposure events.\"\n        },\n        \"ruleID\": {\n          \"type\": \"string\",\n          \"description\": \"The rule\
  \ that matched during evaluation.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The entity type for config_change events (e.g., Gate, Experiment, DynamicConfig).\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The entity name for config_change events.\"\n        },\n        \"action\": {\n          \"type\": \"string\",\n          \"description\": \"The action performed for config_change events (e.g., created, updated, deleted).\"\n        }\n      }\n    },\n    \"statsigMetadata\": {\n      \"$ref\": \"#/$defs/StatsigMetadata\"\n    },\n    \"timeUUID\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this event instance, combining timestamp and random components.\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"$defs\": {\n    \"StatsigUser\": {\n      \"type\": \"object\",\n      \"description\": \"The user object representing the end user associated\
  \ with the event.\",\n      \"properties\": {\n        \"userID\": {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier for the user.\",\n          \"minLength\": 1\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"description\": \"The email address of the user.\",\n          \"format\": \"email\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"ip\": {\n          \"type\": \"string\",\n          \"description\": \"The IP address of the user.\"\n        },\n        \"userAgent\": {\n          \"type\": \"string\",\n          \"description\": \"The user agent string.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The two-letter country code of the user.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"locale\": {\n          \"type\": \"string\",\n         \
  \ \"description\": \"The locale identifier for the user.\"\n        },\n        \"appVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the application the user is running.\"\n        },\n        \"custom\": {\n          \"type\": \"object\",\n          \"description\": \"Custom user properties used for targeting rules.\",\n          \"additionalProperties\": true\n        },\n        \"privateAttributes\": {\n          \"type\": \"object\",\n          \"description\": \"Private user attributes used for evaluation but not logged to Statsig servers.\",\n          \"additionalProperties\": true\n        },\n        \"customIDs\": {\n          \"type\": \"object\",\n          \"description\": \"Custom identifier mappings such as companyID, teamID, or other organizational units.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"StatsigMetadata\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Metadata about the SDK that generated the event.\",\n      \"properties\": {\n        \"sdkType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of SDK (e.g., js-client, py-server, react-native, node-server).\"\n        },\n        \"sdkVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the SDK.\"\n        },\n        \"sessionID\": {\n          \"type\": \"string\",\n          \"description\": \"The session identifier for client-side SDKs.\"\n        },\n        \"stableID\": {\n          \"type\": \"string\",\n          \"description\": \"A stable device identifier for anonymous user tracking.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/json-schema/statsig-event-schema.json
tags: []
title: Statsig Event
---
