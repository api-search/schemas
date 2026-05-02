---
description: Represents a LogRocket session recording containing user interactions, network requests, console logs, and errors captured during a user visit.
layout: schema
name: LogRocket Session
properties_list:
- description: Unique identifier for the session recording.
  name: sessionId
  type: string
- description: The LogRocket application or project identifier.
  name: appId
  type: string
- description: The LogRocket organization identifier.
  name: orgId
  type: string
- description: The identified user ID if the user was identified via LogRocket.identify().
  name: userId
  type: string
- description: The email address of the identified user.
  name: userEmail
  type: string
- description: The display name of the identified user.
  name: userName
  type: string
- description: ISO 8601 timestamp when the session recording started.
  name: startTime
  type: string
- description: ISO 8601 timestamp when the session recording ended.
  name: endTime
  type: string
- description: Duration of the session in milliseconds.
  name: duration
  type: integer
- description: The browser name and version detected during the session.
  name: browser
  type: string
- description: The type of device used during the session.
  name: deviceType
  type: string
- description: The operating system detected during the session.
  name: operatingSystem
  type: string
- description: The country from which the session originated.
  name: country
  type: string
- description: The region or state from which the session originated.
  name: region
  type: string
- description: The city from which the session originated.
  name: city
  type: string
- description: The version of the LogRocket SDK that recorded the session.
  name: sdkVersion
  type: string
- description: The application release version set via LogRocket configuration.
  name: release
  type: string
- description: List of page URLs visited during the session.
  name: pagesVisited
  type: array
- description: Number of JavaScript errors captured during the session.
  name: errorCount
  type: integer
- description: Custom user traits attached via LogRocket.identify() or the User Identification API.
  name: traits
  type: object
provider_name: LogRocket
provider_slug: logrocket
schema_file: json-schema/logrocket-session-schema.json
slug: logrocket-session
source_filename: logrocket-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://logrocket.com/schemas/logrocket/session.json\",\n  \"title\": \"LogRocket Session\",\n  \"description\": \"Represents a LogRocket session recording containing user interactions, network requests, console logs, and errors captured during a user visit.\",\n  \"type\": \"object\",\n  \"required\": [\"sessionId\", \"appId\", \"startTime\"],\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the session recording.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The LogRocket application or project identifier.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The LogRocket organization identifier.\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The identified user ID if the user was identified via LogRocket.identify().\"\n\
  \    },\n    \"userEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the identified user.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the identified user.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the session recording started.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the session recording ended.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Duration of the session in milliseconds.\"\n    },\n    \"browser\": {\n      \"type\": \"string\",\n      \"description\": \"The browser name and version detected during the session.\"\n    },\n    \"deviceType\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The type of device used during the session.\",\n      \"enum\": [\"desktop\", \"mobile\", \"tablet\"]\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system detected during the session.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country from which the session originated.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region or state from which the session originated.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city from which the session originated.\"\n    },\n    \"sdkVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the LogRocket SDK that recorded the session.\"\n    },\n    \"release\": {\n      \"type\": \"string\",\n      \"description\": \"The application release version set via LogRocket configuration.\"\n    },\n    \"pagesVisited\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"List of page URLs visited during the session.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"errorCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of JavaScript errors captured during the session.\"\n    },\n    \"traits\": {\n      \"type\": \"object\",\n      \"description\": \"Custom user traits attached via LogRocket.identify() or the User Identification API.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"NetworkRequest\": {\n      \"type\": \"object\",\n      \"description\": \"A network request captured during the session.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the network request.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The HTTP method used for the request.\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"OPTIONS\", \"HEAD\"]\n        },\n        \"statusCode\": {\n          \"type\": \"integer\",\n          \"description\": \"The HTTP status code returned.\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Duration of the request in milliseconds.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the request was initiated.\"\n        }\n      }\n    },\n    \"ConsoleLog\": {\n      \"type\": \"object\",\n      \"description\": \"A console log entry captured during the session.\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"description\": \"The console log level.\",\n          \"enum\": [\"log\", \"info\", \"warn\", \"error\", \"debug\"]\n        },\n\
  \        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"The console log message.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the console log was recorded.\"\n        }\n      }\n    },\n    \"JavaScriptError\": {\n      \"type\": \"object\",\n      \"description\": \"A JavaScript error captured during the session.\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"The error message.\"\n        },\n        \"stack\": {\n          \"type\": \"string\",\n          \"description\": \"The error stack trace.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the error occurred.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"\
  The page URL where the error occurred.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/json-schema/logrocket-session-schema.json
tags:
- Analytics
- Error Monitoring
- Frontend Monitoring
- Observability
- Session Replay
title: LogRocket Session
---
