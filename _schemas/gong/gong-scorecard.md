---
description: Represents a scorecard configuration in the Gong platform, used for evaluating call quality and performance.
layout: schema
name: Gong Scorecard
properties_list:
- description: Unique identifier for the scorecard.
  name: scorecardId
  type: string
- description: Name of the scorecard.
  name: scorecardName
  type: string
- description: Whether the scorecard is currently enabled.
  name: enabled
  type: boolean
- description: The workspace the scorecard belongs to.
  name: workspaceId
  type: string
- description: When the scorecard was created.
  name: created
  type: string
- description: When the scorecard was last updated.
  name: updated
  type: string
- description: List of questions in the scorecard.
  name: questions
  type: array
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-scorecard-schema.json
slug: gong-scorecard
source_filename: gong-scorecard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-scorecard-schema.json\",\n  \"title\": \"Gong Scorecard\",\n  \"description\": \"Represents a scorecard configuration in the Gong platform, used for evaluating call quality and performance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scorecardId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the scorecard.\"\n    },\n    \"scorecardName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the scorecard.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the scorecard is currently enabled.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace the scorecard belongs to.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"When the scorecard was created.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the scorecard was last updated.\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ScorecardQuestion\"\n      },\n      \"description\": \"List of questions in the scorecard.\"\n    }\n  },\n  \"required\": [\"scorecardId\", \"scorecardName\"],\n  \"$defs\": {\n    \"ScorecardQuestion\": {\n      \"type\": \"object\",\n      \"description\": \"A question within a Gong scorecard.\",\n      \"properties\": {\n        \"questionId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the question.\"\n        },\n        \"questionText\": {\n          \"type\": \"string\",\n          \"description\": \"The question text.\"\n        },\n        \"questionType\": {\n          \"type\": \"string\",\n          \"enum\": [\"YesNo\", \"Scale\", \"\
  FreeText\", \"SingleChoice\", \"MultipleChoice\"],\n          \"description\": \"The type of question.\"\n        },\n        \"isRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the question requires an answer.\"\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"value\": {\n                \"type\": \"string\"\n              },\n              \"label\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"description\": \"Available answer options for choice-type questions.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-scorecard-schema.json
tags: []
title: Gong Scorecard
---
