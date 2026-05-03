---
description: A Segment analytics event conforming to the Segment spec. Events flow through the Segment platform and are delivered to configured destinations. Every event must include a type and either a userId or anonymousId.
layout: schema
name: Segment Event
properties_list:
- description: The type of Segment call. Determines the structure and semantics of the event.
  name: type
  type: string
- description: Unique identifier for the user in your database. Required unless anonymousId is provided.
  name: userId
  type: string
- description: A pseudo-unique substitute for a user ID, typically assigned by the Segment library before a user is identified.
  name: anonymousId
  type: string
- description: The name of the action a user performed. Required for track calls.
  name: event
  type: string
- description: The name of the page or screen. Used in page and screen calls.
  name: name
  type: string
- description: A unique identifier for the group or account. Required for group calls.
  name: groupId
  type: string
- description: The previous user ID to merge with userId. Required for alias calls.
  name: previousId
  type: string
- description: A free-form dictionary of properties for the event. Used with track, page, and screen calls.
  name: properties
  type: object
- description: A free-form dictionary of traits for the user or group. Used with identify and group calls.
  name: traits
  type: object
- description: ''
  name: context
  type: object
- description: A dictionary of destination names to boolean or object values that control which destinations receive this event.
  name: integrations
  type: object
- description: ISO 8601 date string for when the event originally occurred.
  name: timestamp
  type: string
- description: ISO 8601 date string for when the event was sent from the client.
  name: sentAt
  type: string
- description: ISO 8601 date string for when Segment received the event.
  name: receivedAt
  type: string
- description: A unique identifier for the message, used for deduplication.
  name: messageId
  type: string
- description: The source write key. Included in pixel tracking API calls.
  name: writeKey
  type: string
provider_name: segment
provider_slug: segment
schema_file: json-schema/segment-event-schema.json
slug: segment-event
source_filename: segment-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://segment.com/schemas/segment/event.json\",\n  \"title\": \"Segment Event\",\n  \"description\": \"A Segment analytics event conforming to the Segment spec. Events flow through the Segment platform and are delivered to configured destinations. Every event must include a type and either a userId or anonymousId.\",\n  \"type\": \"object\",\n  \"required\": [\"type\"],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Segment call. Determines the structure and semantics of the event.\",\n      \"enum\": [\"identify\", \"track\", \"page\", \"screen\", \"group\", \"alias\"]\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user in your database. Required unless anonymousId is provided.\",\n      \"minLength\": 1\n    },\n    \"anonymousId\": {\n      \"type\": \"string\",\n      \"\
  description\": \"A pseudo-unique substitute for a user ID, typically assigned by the Segment library before a user is identified.\",\n      \"minLength\": 1\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the action a user performed. Required for track calls.\",\n      \"minLength\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the page or screen. Used in page and screen calls.\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the group or account. Required for group calls.\",\n      \"minLength\": 1\n    },\n    \"previousId\": {\n      \"type\": \"string\",\n      \"description\": \"The previous user ID to merge with userId. Required for alias calls.\",\n      \"minLength\": 1\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"A free-form dictionary of properties for the event. Used with track, page,\
  \ and screen calls.\",\n      \"additionalProperties\": true\n    },\n    \"traits\": {\n      \"type\": \"object\",\n      \"description\": \"A free-form dictionary of traits for the user or group. Used with identify and group calls.\",\n      \"additionalProperties\": true\n    },\n    \"context\": {\n      \"$ref\": \"#/$defs/Context\"\n    },\n    \"integrations\": {\n      \"type\": \"object\",\n      \"description\": \"A dictionary of destination names to boolean or object values that control which destinations receive this event.\",\n      \"additionalProperties\": true\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 date string for when the event originally occurred.\"\n    },\n    \"sentAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 date string for when the event was sent from the client.\"\n    },\n    \"receivedAt\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 date string for when Segment received the event.\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the message, used for deduplication.\"\n    },\n    \"writeKey\": {\n      \"type\": \"string\",\n      \"description\": \"The source write key. Included in pixel tracking API calls.\"\n    }\n  },\n  \"anyOf\": [\n    { \"required\": [\"userId\"] },\n    { \"required\": [\"anonymousId\"] }\n  ],\n  \"if\": {\n    \"properties\": { \"type\": { \"const\": \"track\" } }\n  },\n  \"then\": {\n    \"required\": [\"event\"]\n  },\n  \"$defs\": {\n    \"Context\": {\n      \"type\": \"object\",\n      \"description\": \"Contextual information that provides extra details about the event, such as device information, IP address, locale, and library version.\",\n      \"properties\": {\n        \"active\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether the user is currently active.\"\n        },\n        \"ip\": {\n          \"type\": \"string\",\n          \"format\": \"ipv4\",\n          \"description\": \"The IP address of the user.\"\n        },\n        \"locale\": {\n          \"type\": \"string\",\n          \"description\": \"The locale of the user, such as en-US.\",\n          \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\"\n        },\n        \"userAgent\": {\n          \"type\": \"string\",\n          \"description\": \"The user agent string of the client.\"\n        },\n        \"library\": {\n          \"$ref\": \"#/$defs/Library\"\n        },\n        \"page\": {\n          \"$ref\": \"#/$defs/PageContext\"\n        },\n        \"device\": {\n          \"$ref\": \"#/$defs/Device\"\n        },\n        \"os\": {\n          \"$ref\": \"#/$defs/OperatingSystem\"\n        },\n        \"screen\": {\n          \"$ref\": \"#/$defs/Screen\"\n        },\n        \"campaign\": {\n          \"$ref\": \"#/$defs/Campaign\"\n  \
  \      },\n        \"referrer\": {\n          \"type\": \"object\",\n          \"description\": \"Referrer information.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The referrer type.\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The referrer name.\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The referrer URL.\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The referrer link.\"\n            }\n          }\n        },\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The user's timezone, such as America/New_York.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"Library\":\
  \ {\n      \"type\": \"object\",\n      \"description\": \"Information about the Segment library that generated the event.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the Segment library.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the Segment library.\"\n        }\n      }\n    },\n    \"PageContext\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the current web page.\",\n      \"properties\": {\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"The path of the page URL.\"\n        },\n        \"referrer\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The referrer URL.\"\n        },\n        \"search\": {\n          \"type\": \"string\",\n          \"description\": \"The search query string.\"\n        },\n        \"title\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The page title.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The full page URL.\"\n        }\n      }\n    },\n    \"Device\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the user's device.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The device ID.\"\n        },\n        \"advertisingId\": {\n          \"type\": \"string\",\n          \"description\": \"The advertising ID.\"\n        },\n        \"adTrackingEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether ad tracking is enabled.\"\n        },\n        \"manufacturer\": {\n          \"type\": \"string\",\n          \"description\": \"The device manufacturer.\"\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ device model.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The device name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The device type, such as ios or android.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"The push notification token.\"\n        }\n      }\n    },\n    \"OperatingSystem\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the device operating system.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The OS name.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The OS version.\"\n        }\n      }\n    },\n    \"Screen\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the device screen.\",\n      \"properties\": {\n        \"width\": {\n       \
  \   \"type\": \"integer\",\n          \"description\": \"The screen width in pixels.\",\n          \"minimum\": 0\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"The screen height in pixels.\",\n          \"minimum\": 0\n        },\n        \"density\": {\n          \"type\": \"number\",\n          \"description\": \"The screen pixel density.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"Campaign\": {\n      \"type\": \"object\",\n      \"description\": \"Campaign attribution information from UTM parameters.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The campaign name (utm_campaign).\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The campaign source (utm_source).\"\n        },\n        \"medium\": {\n          \"type\": \"string\",\n          \"description\": \"The campaign medium (utm_medium).\"\n\
  \        },\n        \"term\": {\n          \"type\": \"string\",\n          \"description\": \"The campaign term (utm_term).\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The campaign content (utm_content).\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/json-schema/segment-event-schema.json
tags: []
title: Segment Event
---
