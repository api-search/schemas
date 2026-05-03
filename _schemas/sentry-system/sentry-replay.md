---
description: Represents a session replay in Sentry. Replays are recorded user sessions that capture DOM interactions, network requests, and console output, providing video-like playback of user experiences that led to errors.
layout: schema
name: Sentry Replay
properties_list:
- description: The unique identifier of the replay.
  name: id
  type: string
- description: The title of the replay, typically the page URL.
  name: title
  type: string
- description: The project ID the replay belongs to.
  name: projectId
  type: string
- description: Duration of the replay in seconds.
  name: duration
  type: integer
- description: Number of errors that occurred during the replay.
  name: countErrors
  type: integer
- description: Number of recording segments.
  name: countSegments
  type: integer
- description: Number of unique URLs visited during the replay.
  name: countUrls
  type: integer
- description: When the replay session started.
  name: startedAt
  type: string
- description: When the replay session ended.
  name: finishedAt
  type: string
- description: The platform (e.g., javascript).
  name: platform
  type: string
- description: The environment the replay was recorded in.
  name: environment
  type: string
- description: URLs visited during the replay.
  name: urls
  type: array
- description: Information about the user whose session was recorded.
  name: user
  type: object
- description: Browser information.
  name: browser
  type: object
- description: Operating system information.
  name: os
  type: object
- description: Device information.
  name: device
  type: object
- description: Tags associated with the replay.
  name: tags
  type: object
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-replay-schema.json
slug: sentry-replay
source_filename: sentry-replay-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/replay.json\",\n  \"title\": \"Sentry Replay\",\n  \"description\": \"Represents a session replay in Sentry. Replays are recorded user sessions that capture DOM interactions, network requests, and console output, providing video-like playback of user experiences that led to errors.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the replay.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the replay, typically the page URL.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID the replay belongs to.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of the replay in seconds.\"\n    },\n    \"countErrors\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Number of errors that occurred during the replay.\"\n    },\n    \"countSegments\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of recording segments.\"\n    },\n    \"countUrls\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique URLs visited during the replay.\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the replay session started.\"\n    },\n    \"finishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the replay session ended.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform (e.g., javascript).\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The environment the replay was recorded in.\"\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"URLs visited during the replay.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"user\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the user whose session was recorded.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"type\": \"string\"\n        },\n        \"ip_address\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"browser\": {\n      \"type\": \"object\",\n      \"description\": \"Browser information.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"os\": {\n      \"type\": \"object\",\n      \"description\": \"Operating system information.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n  \
  \      },\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"device\": {\n      \"type\": \"object\",\n      \"description\": \"Device information.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"brand\": {\n          \"type\": \"string\"\n        },\n        \"model\": {\n          \"type\": \"string\"\n        },\n        \"family\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags associated with the replay.\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"startedAt\", \"finishedAt\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-replay-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Replay
---
