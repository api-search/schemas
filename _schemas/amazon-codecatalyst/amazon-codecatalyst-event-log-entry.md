---
description: Information about an entry in an event log of Amazon CodeCatalyst activity.
layout: schema
name: EventLogEntry
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: eventName
  type: object
- description: ''
  name: eventType
  type: object
- description: ''
  name: eventCategory
  type: object
- description: ''
  name: eventSource
  type: object
- description: ''
  name: eventTime
  type: object
- description: ''
  name: operationType
  type: object
- description: ''
  name: userIdentity
  type: object
- description: ''
  name: projectInformation
  type: object
- description: ''
  name: requestId
  type: object
- description: ''
  name: requestPayload
  type: object
- description: ''
  name: responsePayload
  type: object
- description: ''
  name: errorCode
  type: object
- description: ''
  name: sourceIpAddress
  type: object
- description: ''
  name: userAgent
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-event-log-entry-schema.json
slug: amazon-codecatalyst-event-log-entry
source_filename: amazon-codecatalyst-event-log-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-event-log-entry-schema.json\",\n  \"title\": \"EventLogEntry\",\n  \"description\": \"Information about an entry in an event log of Amazon CodeCatalyst activity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the event.\"\n        }\n      ]\n    },\n    \"eventName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the event.\"\n        }\n      ]\n    },\n    \"eventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n        \
  \  \"description\": \"The type of the event.\"\n        }\n      ]\n    },\n    \"eventCategory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The category for the event.\"\n        }\n      ]\n    },\n    \"eventSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The source of the event.\"\n        }\n      ]\n    },\n    \"eventTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The time the event took place, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    },\n    \"operationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperationType\"\
  \n        },\n        {\n          \"description\": \"The type of the event.\"\n        }\n      ]\n    },\n    \"userIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdentity\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the user whose actions are recorded in the event.\"\n        }\n      ]\n    },\n    \"projectInformation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectInformation\"\n        },\n        {\n          \"description\": \"Information about the project where the event occurred.\"\n        }\n      ]\n    },\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the request.\"\n        }\n      ]\n    },\n    \"requestPayload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventPayload\"\
  \n        },\n        {\n          \"description\": \"Information about the payload of the request.\"\n        }\n      ]\n    },\n    \"responsePayload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventPayload\"\n        },\n        {\n          \"description\": \"Information about the payload of the response, if any.\"\n        }\n      ]\n    },\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The code of the error, if any.\"\n        }\n      ]\n    },\n    \"sourceIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The IP address of the user whose actions are recorded in the event.\"\n        }\n      ]\n    },\n    \"userAgent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n\
  \          \"description\": \"The user agent whose actions are recorded in the event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"eventName\",\n    \"eventType\",\n    \"eventCategory\",\n    \"eventSource\",\n    \"eventTime\",\n    \"operationType\",\n    \"userIdentity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-event-log-entry-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: EventLogEntry
---
