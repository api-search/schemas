---
description: Represents a change data capture event emitted by Fauna event sources. Events are generated when tracked changes occur in a database and are delivered via event streams (real-time) or event feeds (polling). Each event includes the change type, transaction timestamp, cursor for pagination and reconnection, and the associated document data.
layout: schema
name: Fauna Event
properties_list:
- description: The type of change event. 'add' indicates a document was added to the tracked set, 'remove' indicates removal, 'update' indicates modification, and 'status' is a heartbeat or connection status event.
  name: type
  type: string
- description: Transaction timestamp in microseconds since the Unix epoch when the change occurred.
  name: txn_ts
  type: integer
- description: Cursor position for this event. Used for pagination in event feeds and for reconnection in event streams.
  name: cursor
  type: string
- description: The document data associated with the event. Present for add, remove, and update events. The structure depends on the collection schema.
  name: data
  type: object
- description: ''
  name: stats
  type: object
provider_name: fauna
provider_slug: fauna
schema_file: json-schema/fauna-event-schema.json
slug: fauna-event
source_filename: fauna-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fauna.com/schemas/fauna/event.json\",\n  \"title\": \"Fauna Event\",\n  \"description\": \"Represents a change data capture event emitted by Fauna event sources. Events are generated when tracked changes occur in a database and are delivered via event streams (real-time) or event feeds (polling). Each event includes the change type, transaction timestamp, cursor for pagination and reconnection, and the associated document data.\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"txn_ts\"],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"add\", \"remove\", \"update\", \"status\"],\n      \"description\": \"The type of change event. 'add' indicates a document was added to the tracked set, 'remove' indicates removal, 'update' indicates modification, and 'status' is a heartbeat or connection status event.\"\n    },\n    \"txn_ts\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Transaction timestamp in microseconds since the Unix epoch when the change occurred.\"\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor position for this event. Used for pagination in event feeds and for reconnection in event streams.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The document data associated with the event. Present for add, remove, and update events. The structure depends on the collection schema.\"\n    },\n    \"stats\": {\n      \"$ref\": \"#/$defs/EventStats\"\n    }\n  },\n  \"$defs\": {\n    \"EventStats\": {\n      \"type\": \"object\",\n      \"description\": \"Operational statistics for the event processing.\",\n      \"properties\": {\n        \"read_ops\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of Transactional Read Operations consumed.\"\n        },\n        \"storage_bytes_read\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Number of bytes read from storage.\"\n        },\n        \"compute_ops\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of Transactional Compute Operations consumed.\"\n        },\n        \"processing_time_ms\": {\n          \"type\": \"integer\",\n          \"description\": \"Processing time in milliseconds.\"\n        },\n        \"rate_limits_hit\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of rate limits that were hit during event processing.\"\n        }\n      }\n    },\n    \"EventFeedPage\": {\n      \"type\": \"object\",\n      \"description\": \"A page of events returned by the event feed endpoint.\",\n      \"required\": [\"events\", \"has_next\"],\n      \"properties\": {\n        \"events\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#\"\n \
  \         },\n          \"description\": \"Array of change events for the current page.\"\n        },\n        \"cursor\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor to use for fetching the next page of events.\"\n        },\n        \"has_next\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether more pages of events are available.\"\n        },\n        \"stats\": {\n          \"$ref\": \"#/$defs/EventStats\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/json-schema/fauna-event-schema.json
tags: []
title: Fauna Event
---
