---
description: Represents a tracked event in Mixpanel, capturing a user action with associated properties including timing, identity, and custom attributes.
layout: schema
name: Mixpanel Event
properties_list:
- description: The name of the event (e.g., 'Sign Up', 'Purchase', 'Page View')
  name: event
  type: string
- description: Properties associated with the event
  name: properties
  type: object
provider_name: Mixpanel
provider_slug: mixpanel
schema_file: json-schema/mixpanel-event-schema.json
slug: mixpanel-event
source_filename: mixpanel-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.mixpanel.com/schemas/mixpanel/event.json\",\n  \"title\": \"Mixpanel Event\",\n  \"description\": \"Represents a tracked event in Mixpanel, capturing a user action with associated properties including timing, identity, and custom attributes.\",\n  \"type\": \"object\",\n  \"required\": [\"event\", \"properties\"],\n  \"properties\": {\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event (e.g., 'Sign Up', 'Purchase', 'Page View')\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties associated with the event\",\n      \"properties\": {\n        \"distinct_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the user who performed the event\"\n        },\n        \"time\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Unix timestamp in seconds when the event occurred\"\n        },\n        \"$insert_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the event used for deduplication\",\n          \"maxLength\": 36\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Mixpanel project token\"\n        },\n        \"$device_id\": {\n          \"type\": \"string\",\n          \"description\": \"Anonymous device identifier\"\n        },\n        \"$user_id\": {\n          \"type\": \"string\",\n          \"description\": \"Authenticated user identifier\"\n        },\n        \"mp_country_code\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter country code derived from IP geolocation\"\n        },\n        \"$city\": {\n          \"type\": \"string\",\n          \"description\": \"City derived from IP geolocation\"\n        },\n        \"$region\": {\n          \"\
  type\": \"string\",\n          \"description\": \"Region or state derived from IP geolocation\"\n        },\n        \"$browser\": {\n          \"type\": \"string\",\n          \"description\": \"Browser name (e.g., Chrome, Safari, Firefox)\"\n        },\n        \"$os\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system name\"\n        },\n        \"$current_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the page where the event occurred\"\n        },\n        \"$referrer\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Referring URL\"\n        },\n        \"$screen_height\": {\n          \"type\": \"integer\",\n          \"description\": \"Screen height in pixels\"\n        },\n        \"$screen_width\": {\n          \"type\": \"integer\",\n          \"description\": \"Screen width in pixels\"\n        },\n        \"mp_lib\": {\n         \
  \ \"type\": \"string\",\n          \"description\": \"Mixpanel SDK library name and version\"\n        }\n      },\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/json-schema/mixpanel-event-schema.json
tags:
- Analytics
- Data Analysis
- Event Tracking
- Product Analytics
- User Behavior
title: Mixpanel Event
---
