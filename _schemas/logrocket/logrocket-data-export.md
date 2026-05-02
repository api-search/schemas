---
description: Represents a line in the JSON Lines file produced by the LogRocket data export. Each line contains a session event with metadata, user information, and event-specific data.
layout: schema
name: LogRocket Data Export Record
properties_list:
- description: The type of event recorded, such as lr.Metadata, network request, console log, or DOM mutation.
  name: eventType
  type: string
- description: Unix timestamp in milliseconds when the event occurred.
  name: timestamp
  type: integer
- description: Unique identifier for the session this event belongs to.
  name: sessionId
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: user
  type: object
- description: ''
  name: network
  type: object
- description: ''
  name: console
  type: object
- description: ''
  name: error
  type: object
provider_name: LogRocket
provider_slug: logrocket
schema_file: json-schema/logrocket-data-export-schema.json
slug: logrocket-data-export
source_filename: logrocket-data-export-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://logrocket.com/schemas/logrocket/data-export.json\",\n  \"title\": \"LogRocket Data Export Record\",\n  \"description\": \"Represents a line in the JSON Lines file produced by the LogRocket data export. Each line contains a session event with metadata, user information, and event-specific data.\",\n  \"type\": \"object\",\n  \"required\": [\"eventType\", \"timestamp\"],\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event recorded, such as lr.Metadata, network request, console log, or DOM mutation.\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in milliseconds when the event occurred.\"\n    },\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the session this event belongs to.\"\n    },\n  \
  \  \"metadata\": {\n      \"$ref\": \"#/$defs/SessionMetadata\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/UserInfo\"\n    },\n    \"network\": {\n      \"$ref\": \"#/$defs/NetworkEvent\"\n    },\n    \"console\": {\n      \"$ref\": \"#/$defs/ConsoleEvent\"\n    },\n    \"error\": {\n      \"$ref\": \"#/$defs/ErrorEvent\"\n    }\n  },\n  \"$defs\": {\n    \"SessionMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the session including browser, device, location, and SDK information.\",\n      \"properties\": {\n        \"release\": {\n          \"type\": \"string\",\n          \"description\": \"The application release version.\"\n        },\n        \"sdkVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The LogRocket SDK version that captured this session.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The country from which the session originated.\"\n        },\n\
  \        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"The region or state from which the session originated.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city from which the session originated.\"\n        },\n        \"browser\": {\n          \"type\": \"string\",\n          \"description\": \"The browser name and version.\"\n        },\n        \"browserVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The browser version string.\"\n        },\n        \"deviceType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of device.\"\n        }\n      }\n    },\n    \"UserInfo\": {\n      \"type\": \"object\",\n      \"description\": \"User identification data from LogRocket.identify() calls or anonymous session identifiers.\",\n      \"properties\": {\n        \"userId\": {\n          \"type\": \"string\",\n          \"description\": \"The identified\
  \ user ID or auto-generated anonymous identifier.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the identified user.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the identified user.\"\n        },\n        \"traits\": {\n          \"type\": \"object\",\n          \"description\": \"Custom user traits.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"NetworkEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A network request or response event.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the network request.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"The HTTP\
  \ method.\"\n        },\n        \"statusCode\": {\n          \"type\": \"integer\",\n          \"description\": \"The HTTP response status code.\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Request duration in milliseconds.\"\n        }\n      }\n    },\n    \"ConsoleEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A console log event.\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"description\": \"The console log level.\",\n          \"enum\": [\"log\", \"info\", \"warn\", \"error\", \"debug\"]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"The console log message content.\"\n        }\n      }\n    },\n    \"ErrorEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A JavaScript error event.\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The error message.\"\n        },\n        \"stack\": {\n          \"type\": \"string\",\n          \"description\": \"The error stack trace.\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The source file where the error originated.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/json-schema/logrocket-data-export-schema.json
tags:
- Analytics
- Error Monitoring
- Frontend Monitoring
- Observability
- Session Replay
title: LogRocket Data Export Record
---
