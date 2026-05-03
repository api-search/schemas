---
description: Represents a question asked across managed endpoints in the Tanium platform. Questions are the primary mechanism for collecting real-time data from endpoints using sensors.
layout: schema
name: Tanium Question
properties_list:
- description: Unique numeric identifier for the question
  name: id
  type: integer
- description: Human-readable question text
  name: queryText
  type: string
- description: Timestamp when the question expires and stops collecting results
  name: expiration
  type: string
- description: List of sensors selected for the question
  name: selects
  type: array
- description: Target group filter restricting which endpoints answer
  name: group
  type: object
- description: Management rights group for access control
  name: managementRightsGroup
  type: object
- description: Reference to an associated saved question
  name: savedQuestion
  type: object
provider_name: Tanium
provider_slug: tanium
schema_file: json-schema/tanium-question-schema.json
slug: tanium-question
source_filename: tanium-question-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/tanium/blob/main/json-schema/tanium-question-schema.json\",\n  \"title\": \"Tanium Question\",\n  \"description\": \"Represents a question asked across managed endpoints in the Tanium platform. Questions are the primary mechanism for collecting real-time data from endpoints using sensors.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the question\"\n    },\n    \"queryText\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable question text\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the question expires and stops collecting results\"\n    },\n    \"selects\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n     \
  \   \"properties\": {\n          \"sensor\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Sensor name\"\n              },\n              \"hash\": {\n                \"type\": \"integer\",\n                \"description\": \"Sensor hash identifier\"\n              },\n              \"id\": {\n                \"type\": \"integer\",\n                \"description\": \"Sensor numeric identifier\"\n              }\n            },\n            \"description\": \"Sensor used for data collection\"\n          }\n        }\n      },\n      \"description\": \"List of sensors selected for the question\"\n    },\n    \"group\": {\n      \"$ref\": \"#/$defs/GroupFilter\",\n      \"description\": \"Target group filter restricting which endpoints answer\"\n    },\n    \"managementRightsGroup\": {\n      \"$ref\": \"#/$defs/GroupFilter\",\n      \"description\": \"Management rights\
  \ group for access control\"\n    },\n    \"savedQuestion\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Associated saved question identifier\"\n        }\n      },\n      \"description\": \"Reference to an associated saved question\"\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"GroupFilter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Group identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Group name\"\n        },\n        \"andFlag\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether filters are combined with AND logic\"\n        },\n        \"filters\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"sensor\"\
  : {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\"\n                  },\n                  \"hash\": {\n                    \"type\": \"integer\"\n                  }\n                }\n              },\n              \"operator\": {\n                \"type\": \"string\",\n                \"description\": \"Filter operator (e.g., RegexMatch, Contains, Equal)\"\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"Filter value\"\n              }\n            }\n          },\n          \"description\": \"Filter criteria for group membership\"\n        }\n      },\n      \"description\": \"A group filter definition used for targeting endpoints\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/json-schema/tanium-question-schema.json
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
title: Tanium Question
---
